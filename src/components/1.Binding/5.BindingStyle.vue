<template>
  <div>
    <!-- Memasukkan inline style yang sudah dibuat di komponen vue dan memasukkan nya ke dalam HTML -->
    <h1
      v-bind:style="{
        color: textGreen,
        fontSize: fontSize + 'px',
        padding: '20px',
      }"
    >
      Inline Style
    </h1>

    <!-- Memasukkan object css sekaligus dalam 1 komponen vue js dan memasukkan ke dalam HTML -->
    <h1 v-bind:style="styleObject">Inline Style</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      textGreen: 'green',
      fontSize: 50,
      styleObject: {
        color: 'green',
        fontSize: '50px',
        padding: '20px',
      },
    };
  },
};
</script>
