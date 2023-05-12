<!-- Todo -->
<!-- Conditional rendering di Vue.js adalah teknik untuk menampilkan atau menyembunyikan elemen HTML atau komponen Vue.js berdasarkan kondisi tertentu. Dalam Vue.js, kondisi tersebut bisa diatur melalui penggunaan direktif v-if atau v-show. -->

<template>
  <div>
    <!-- Ini cara pembuatan kodisi di vue js , dimana jika number sama dengan 0 maka tampilkan HTML nya dan jika tidak maka jangan tampilkan HTML nya -->
    <h1 v-if="number === 0" class="text-green-400 font-semibold text-2xl">
      Ini adalah nomor 0
    </h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
    };
  },
};
</script>

<style lang="scss" scoped></style>
