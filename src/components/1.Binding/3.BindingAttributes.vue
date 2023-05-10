<!-- Todo -->
<!-- Binding Attributes di Vue.js adalah salah satu jenis binding yang digunakan untuk mamasukkan nilai atribut dari properti objek Vue ke dalam atribut elemen HTML. -->

<template>
  <div class="border border-green-400">
    <h2 v-bind:id="headerId" class="text-green-500 text-2xl">Header</h2>
    <button
      v-bind:disabled="isDisabled"
      class="py-4 px-10 bg-green-600 text-white font-semibold rounded-md"
    >
      Submit
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      headerId: 'Header',
      isDisabled: true,
    };
  },
};
</script>
