<!-- Todo -->
<!-- Binding HTML di Vue.js adalah salah satu jenis binding yang digunakan untuk menampilkan konten HTML yang dihasilkan secara dinamis dari objek Vue ke dalam elemen HTML. -->

<template>
  <div>
    <h1 v-html="name" class="text-green-500 text-2xl"></h1>
    <p v-html="nim" class="text-green-500 text-2xl font-semibold"></p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: '<b> Thomas Alberto </b>', // Binding HTML
      nim: '<q> 12221355 </q>', // Binding HTMl
    };
  },
};
</script>

<style lang="scss" scoped></style>
