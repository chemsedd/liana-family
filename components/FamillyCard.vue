<template>
  <div class="card">
    <a
      :href="`https://online.heredis.com/fr/search/?name=${name}&firstname=&place=`"
      target="_blank"
      >{{ name }}
    </a>
  </div>
</template>

<script>
export default {
  props: ["name"],
};
</script>

<style>
.card {
  @apply flex flex-col items-center;
  @apply text-white font-semibold uppercase;
  @apply bg-green-400 rounded-md shadow-md p-8;
  @apply hover:bg-green-500;
}

.card a {
  @apply w-full h-full;
}
</style>