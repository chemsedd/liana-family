<template>
  <header class="header-container">
    <a href="/" class="font-bold uppercase text-2xl">Familles de Liana</a>
    <h2>Rechercher un arbre généalogique des familles de Liana</h2>
  </header>
</template>

<script>
export default {};
</script>

<style>
.header-container {
  @apply flex flex-col gap-y-4;
  @apply md:flex-row md:justify-between md:items-center;
  @apply py-4 px-16 md:px-20 w-full;
  @apply bg-green-800 bg-opacity-90 text-gray-100;
}
</style>