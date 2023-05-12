<!-- Todo -->
<!-- Conditional list rendering adalah teknik dalam Vue.js untuk melakukan list rendering berdasarkan kondisi atau filter tertentu. Dengan menggunakan conditional list rendering, kita dapat menampilkan hanya elemen list yang memenuhi kondisi tertentu atau melakukan filter terhadap elemen list yang akan ditampilkan. -->

<template>
  <template v-for="name in names" :key="name">
    <h2 v-if="name === 'Thomas'" class="text-green-400 font-semibold text-2xl">
      {{ name }}
    </h2>
  </template>
</template>

<script>
export default {
  data() {
    return {
      names: ['Thomas', 'Frans', 'Teguh'],
    };
  },
};
</script>
