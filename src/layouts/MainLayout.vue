<template>
  <div>Main layout</div>
  <RouterView v-slot="{ Component }">
    <transition name="fade" mode="out-in">
      <component :is="Component" :key="$route.path"></component>
    </transition>
  </RouterView>
</template>

<script setup></script>

<style lang="scss" scoped></style>
