<!-- Todo -->
<!-- List rendering di Vue.js adalah cara untuk menampilkan daftar item atau data yang dinamis pada halaman web. List rendering dapat dilakukan dengan menggunakan directive v-for di dalam elemen HTML atau komponen Vue.js. -->

<template>
  <div>
    <!-- <ListRendering /> -->
    <!-- <ListAndKey /> -->
    <ConditionalList />
  </div>
</template>

<script>
import ListRendering from '../components/3.List/1.ListRendering.vue';
import ListAndKey from '../components/3.List/2.ListAndKey.vue';
import ConditionalList from '../components/3.List/3.ConditionalList.vue';

export default {
  components: {
    ListRendering,
    ListAndKey,
    ConditionalList,
  },
};
</script>
