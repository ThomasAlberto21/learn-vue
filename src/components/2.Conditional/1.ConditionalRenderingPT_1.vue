<template>
  <!-- Menggunakan conditional rendering if else if dan else -->
  <div>
    <h1 v-if="number === 0" class="text-green-400 font-semibold text-2xl">
      This is number 0
    </h1>

    <h1 v-else-if="number > 0" class="text-green-400 font-semibold text-2xl">
      The number positive
    </h1>

    <h1 v-else-if="number < 0" class="text-green-400 font-semibold text-2xl">
      The number negative
    </h1>

    <h1 v-else class="text-green-400 font-semibold text-2xl">Is not number</h1>
  </div>

  <!-- Template tag dalam conditional rendering di Vue.js berguna untuk mengelompokkan beberapa elemen HTML atau komponen Vue.js dalam satu blok dan diterapkan juga kondisi pada blok tersebut  -->
  <template v-if="shodHeader">
    <h1 class="text-green-400 font-semibold text-2xl">Ini adalah Header</h1>
    <p class="text-orange-400 text-lg">Ini adalah text header</p>
  </template>

  <template v-if="showFooter">
    <h1 class="text-green-400 font-semibold text-2xl">Ini adalah Footer</h1>
    <p class="text-orange-400 text-lg">Ini adalah text footer</p>
  </template>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
      shodHeader: false,
      showFooter: true,
    };
  },
};
</script>
