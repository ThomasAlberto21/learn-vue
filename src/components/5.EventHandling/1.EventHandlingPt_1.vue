<template>
  <div class="text-center">
    <h1 class="text-2xl text-green-500 font-semibold">{{ name }}</h1>
    <button
      v-on:click="name = 'Fransiskus Berto'"
      class="px-3 py-2 bg-green-500 rounded-lg mx-2"
    >
      Fransiskus Berto
    </button>
    <button
      v-on:click="name = 'Teguh Firmansyah'"
      class="px-3 py-2 bg-green-500 rounded-lg"
    >
      Teguh Firmansyah
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Thomas Alberto',
    };
  },
};
</script>
