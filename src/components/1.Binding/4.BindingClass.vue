<!-- Todo -->
<!-- Binding class di Vue.js adalah direktif yang digunakan untuk memasukkan nilai dari atribut class pada elemen HTML yang data nya diambil di komponen Vue -->

<template>
  <div>
    <h1 v-bind:class="status">Underline</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      status: 'text-green-400 font-bold text-2xl',
    };
  },
};
</script>
