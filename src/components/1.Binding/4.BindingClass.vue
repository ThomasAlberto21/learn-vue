<!-- Todo -->
<!-- Binding class di Vue.js adalah direktif yang digunakan untuk memasukkan nilai dari atribut class pada elemen HTML yang data nya diambil di komponen Vue -->

<template>
  <div>
    <!-- Memasukkan class yang sudah disediakan di komponen Vue dengan cara v-bind:class-->
    <h1 v-bind:class="status">Penggunaan v-bind:class cara 1</h1>

    <!-- Jika isPromoted true maka jalankan komponen promoted dan jika isPromoted false maka jangan jalankan komponen promoted nya -->
    <h1 v-bind:class="isPromoted && promoted">
      Penggunaan v-bind:class cara 2
    </h1>

    <!-- Jika isSoldout bernilai true maka jalankan komponen soldOut dan jika isSoldout bernilai false maka jalankan komponen promoted nya -->
    <h1 v-bind:class="isSoldout ? soldOut : promoted">
      Penggunaan v-bind:class cara 3
    </h1>

    <!-- Fungsi menggunakan array dalam v-bind:class bertujuan untuk menggabungkan class yang kita miliki di komponen Vue menjadi satu di dalam HTML nya -->
    <h1 v-bind:class="[textSemibold, textGreen, text2xl]">
      Penggunaan v-bind:class cara 4
    </h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      status: 'text-green-400 font-semibold text-2xl',
      isPromoted: true,
      promoted: 'text-green-400 font-semibold text-2xl',
      isSoldout: false,
      soldOut: 'text-red-600 font-semibold text-2xl',
      textSemibold: 'font-semibold',
      text2xl: 'text-2xl',
      textGreen: 'text-green-400',
    };
  },
};
</script>

<style></style>
