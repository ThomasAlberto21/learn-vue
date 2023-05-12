<!-- Todo -->
<!-- Properti "key" pada list rendering di Vue.js digunakan untuk memberikan identitas unik pada setiap elemen list. Hal ini memungkinkan Vue untuk melakukan optimisasi rendering yang lebih baik ketika elemen list berubah atau di-update. -->

<template>
  <template v-for="name in names" :key="name">
    <h2 class="text-green-400 text-2xl font-semibold">{{ name }}</h2>
    <input placeholder="Last name" class="text-green-400" />
    <hr />
  </template>
  <button
    @click="shuffle"
    class="px-10 py-2 bg-green-600 rounded-lg text-white"
  >
    Shuffle!
  </button>
</template>

<script>
import _ from 'lodash';
export default {
  name: 'App',
  data() {
    return {
      names: ['Bruce', 'Clark', 'Diana', 'Barry'],
    };
  },
  methods: {
    shuffle() {
      console.log(this.names);
      this.names = _.shuffle(this.names);
    },
  },
};
</script>
