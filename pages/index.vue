<template>
  <main class="main-container">
    <h1>Familles de Liana</h1>
    <input type="text" name="name" id="name" />
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
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.main-container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}
</style>