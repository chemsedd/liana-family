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
  @apply inline-flex items-center text-center;
  @apply text-gray-700 font-semibold uppercase;
  @apply bg-gray-50 rounded-full shadow-md px-8 py-2;
  @apply hover:bg-gray-300;
}

.card a {
  @apply w-full h-full;
}
</style>