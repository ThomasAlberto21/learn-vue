<!-- Todo -->
<!-- Binding Text di Vue.js adalah salah satu jenis binding yang digunakan untuk menampilkan nilai dari objek Vue ke dalam teks di dalam elemen HTML. -->

<template>
  <!-- Cara 1 menggunakan double curly braces -->
  <h1 class="text-green-500 text-2xl font-semibold">
    Hello My Name Is {{ name }}
  </h1>

  <!-- Cara 2 menggunakan v-text -->
  <p v-text="nim" class="text-green-500 text-2xl font-semibold"></p>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'Thomas Alberto',
      nim: '12221355',
    };
  },
};
</script>
