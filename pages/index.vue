<template>
  <main class="main-container">
    <h1 class="text-6xl text-white font-bold capitalize pb-10">
      Familles de Liana
    </h1>
    <p class="text-white text-center">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolore expedita
      aliquid placeat ut fuga laborum eum illum aliquam voluptatum deserunt
      vitae atque, quae corrupti corporis iste magnam sunt laudantium dicta.
    </p>
    <div class="input-container">
      <input
        type="text"
        name="name"
        id="name"
        v-model="name"
        placeholder="Nom de famille"
      /><input
        type="text"
        name="firstname"
        id="firstname"
        v-model="firstname"
        placeholder="Prénom"
      />
      <a
        class="bg-gray-50 py-2 px-4 rounded shadow"
        :href="`https://online.heredis.com/fr/search/?name=${name}&firstname=${firstname}&place=`"
        target="blank"
        >Check</a
      >
    </div>
    <hr class="w-full" />
    <div class="cards-container">
      <familly-card color="green-800" name="senoussi" />
      <familly-card color="blue-800" name="bouzaher" />
      <familly-card color="yellow-800" name="masmoudi" />
      <familly-card color="pink-800" name="bensaid" />
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
  data() {
    return {
      name: "",
      firstname: "",
    };
  },
};
</script>

<style>
main.main-container {
  @apply flex flex-col justify-center items-center gap-4;
  @apply py-20 px-4;
  @apply w-10/12 md:w-8/12 lg:w-1/2;
}

.input-container {
  @apply flex flex-col items-center justify-center gap-4;
  @apply md:flex-row;
}

.cards-container {
  @apply grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-4;
  @apply w-full;
}

input {
  @apply rounded-md px-4 py-2;
  @apply font-semibold;
  @apply placeholder-gray-500 place-content-stretch;
}

input#name {
  @apply uppercase;
}

input#firstname {
  @apply capitalize;
}
</style>