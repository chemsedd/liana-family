<template>
  <div class="app-container relative">
    <div class="app-bg"></div>
    <my-header />
    <Nuxt />
    <my-footer />
  </div>
</template>

<style>
.app-bg {
  background: url(~/assets/liana.jpg);
  filter: brightness(20%);
  @apply absolute bg-cover w-full h-full;
  z-index: -1;
}

.app-container {
  @apply flex flex-col justify-between items-center;
  @apply min-w-full min-h-screen;
}
</style>