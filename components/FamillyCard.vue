<template>
  <div :class="`card bg-${color}`" @click="goToTree()">
    <a
      :href="`https://online.heredis.com/fr/search/?name=${name}&firstname=&place=`"
      target="_blank"
      :ref="`${name}_tree`"
      >{{ name }}
    </a>
  </div>
</template>

<script>
export default {
  props: ["name", "color"],
  methods: {
    goToTree() {
      this.$refs[`${this.name}_tree`].click();
    },
  },
};
</script>

<style>
.card {
  @apply inline-flex items-center text-center;
  @apply text-white font-semibold uppercase;
  @apply rounded-lg shadow-md px-8 py-2 bg-opacity-60;
  @apply hover:bg-opacity-95;
  &:hover {
    @apply ring cursor-pointer;
  }
}

.card a {
  @apply w-full h-full;
}
</style>