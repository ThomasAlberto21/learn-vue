<!-- Todo -->
<!-- Binding HTML di Vue.js adalah salah satu jenis binding yang digunakan untuk menampilkan konten HTML yang dihasilkan secara dinamis dari objek Vue ke dalam elemen HTML. -->

<template>
  <div class="border border-green-400">
    <h1 v-html="name" class="text-green-500 text-2xl"></h1>
    <p v-html="nim" class="text-green-500 text-2xl font-semibold"></p>
    <p v-html="alert" class="text-white text-2xl font-semibold"></p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: '<b> Thomas Alberto </b>', // Binding HTML
      nim: '<q> 12221355 </q>', // Binding HTMl
      alert: `<a href="#" onclick="alert('Tombol sudah ditekan')">Klik Alert</a>`, // Binding HTML
    };
  },
};
</script>
