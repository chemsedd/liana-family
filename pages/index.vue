<template>
  <main class="main-container">
    <h1 class="text-4xl font-bold capitalize">Familles de Liana</h1>
    <div>
      <input type="text" name="name" id="name" />
      <a
        :href="`https://online.heredis.com/fr/search/?name=senoussi&firstname=&place=`"
        target="blank"
        >Check</a
      >
    </div>
    <hr />
    <div class="cards-container">
      <familly-card name="senoussi" />
      <familly-card name="bouzaher" />
      <familly-card name="masmoudi" />
      <familly-card name="khra" />
    </div>
  </main>
</template>

<script>
export default {
  head: {
    title: "Familles de Liana",
    meta: [
      { charset: "utf-8" },
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        hid: "description",
        name: "description",
        content: "my website description",
      },
    ],
    link: [{ rel: "icon", type: "image/x-icon", href: "/favicon.ico" }],
  },
};
</script>

<style>
body {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}

.main-container {
  @apply flex flex-col justify-center items-center gap-4;
}

.cards-container {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(4, minmax(0, 1fr));
  gap: 1rem;
}
</style>