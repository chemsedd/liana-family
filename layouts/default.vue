<template>
  <div class="app-container relative">
    <div class="app-bg"></div>
    <my-header />
    <Nuxt />
    <my-footer />
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

.app-bg {
  background: url(~/assets/liana.jpg);
  filter: brightness(40%);
  @apply absolute bg-cover w-full h-full;
  z-index: -1;
}

.app-container {
  @apply flex flex-col justify-between items-center;
  @apply w-screen h-screen;
}
</style>