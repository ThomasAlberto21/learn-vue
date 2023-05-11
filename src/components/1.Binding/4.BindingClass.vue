<!-- Todo -->
<!-- Binding class di Vue.js adalah direktif yang digunakan untuk memasukkan nilai dari atribut class pada elemen HTML yang data nya diambil di komponen Vue -->

<template>
  <div>
    <h1 v-bind:class="status">Cara 1</h1>

    <!-- Jika isPromoted true maka jalankan class promoted dan jika isPromoted false maka jangan jalankan isPromoted nya -->
    <h2 v-bind:class="isPromoted && 'promoted'">Cara 2</h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      status: 'text-green-400 font-bold text-2xl',
      isPromoted: true,
    };
  },
};
</script>

<style>
.promoted {
  color: aqua;
  font-size: x-large;
}
</style>
