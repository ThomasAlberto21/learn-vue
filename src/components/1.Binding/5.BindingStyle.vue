<template>
  <!-- Memasukkan object css yang sudah dibuat di komponen Vue js dan memasukkan ke dalam HTML -->
  <div v-bind:style="[border, padding]">
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

    <!-- Memasukkan object css sekaligus yang sudah dibuat di komponen Vue js dan memasukkan ke dalam HTML -->
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

      border: {
        border: '2px solid green',
      },

      padding: {
        paddingTop: '20px',
        paddingBottom: '20px',
        paddingLeft: '20px',
        paddingRight: '20px',
      },
    };
  },
};
</script>

<!-- <style>
*{
    pad
}
</style> -->
