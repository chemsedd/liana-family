<template>
  <div class="app-container">
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

.app-container {
  @apply flex flex-col justify-between items-center;
  @apply w-screen h-screen bg-gray-100;
}
</style>