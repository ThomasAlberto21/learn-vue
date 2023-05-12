<!-- Todo -->
<!-- v-show menampilkan atau menyembunyikan elemen HTML atau komponen Vue.js berdasarkan nilai boolean yang diberikan. Saat rendering awal, elemen HTML atau komponen Vue.js akan selalu dirender ke dalam DOM, tetapi ditampilkan atau disembunyikan berdasarkan nilai boolean yang diberikan. Saat kondisi berubah, elemen HTML atau komponen Vue.js tetap ada di dalam DOM dan hanya ditampilkan atau disembunyikan sesuai dengan kondisi terbaru -->

<!-- v-if menampilkan atau tidak menampilkan elemen HTML atau komponen Vue.js berdasarkan kondisi tertentu. Saat rendering awal, elemen HTML atau komponen Vue.js hanya akan dirender ke dalam DOM jika kondisi benar. Saat kondisi berubah, elemen HTML atau komponen Vue.js akan dihapus dari DOM jika kondisi tidak benar dan ditambahkan ke dalam DOM jika kondisi benar. -->

<!-- Karena v-show hanya menyembunyikan atau menampilkan elemen HTML atau komponen Vue.js dan tidak menghapusnya dari DOM, v-show biasanya lebih cepat daripada v-if saat kondisi berubah secara berkala. Namun, jika kondisi jarang berubah dan elemen HTML atau komponen Vue.js sangat kompleks, v-if dapat lebih efisien dalam hal performa karena elemen HTML atau komponen Vue.js dihapus dari DOM ketika kondisi tidak benar. -->

<template>
  <div>
    <h1 v-show="showElement" class="text-green-400 font-semibold text-2xl">
      Using v-show
    </h1>

    <h1 v-if="showElement" class="text-green-400 font-semibold text-2xl">
      Using v-if
    </h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showElement: true,
    };
  },
};
</script>
