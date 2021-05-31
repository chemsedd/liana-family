<template>
  <header class="header-container">
    <a href="/" class="font-bold uppercase text-2xl">Liana</a>
    <ul class="header-links">
      <li>Acceuil</li>
      <li>About</li>
    </ul>
  </header>
</template>

<script>
export default {};
</script>

<style>
.header-container {
  @apply flex justify-between items-center;
  @apply py-4 px-20 w-full;
  @apply bg-gray-900 text-gray-100;
}

.header-links {
  @apply flex justify-end items-center gap-4;
}

ul.header-links li {
  @apply font-bold;
}
</style>