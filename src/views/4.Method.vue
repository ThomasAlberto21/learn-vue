<template>
  <div>
    <h1 class="text-2xl text-green-400">Menggunakan Cara 1 : {{ add_1() }}</h1>
    <h1 class="text-2xl text-green-400">
      Menggunakan Cara 2 : {{ add_1(2, 3, 5) }}
    </h1>
    <h1 class="text-2xl text-green-400">
      Memasukkan data ke dalam methods : {{ multiply(10) }}
    </h1>

    <h1 class="text-2xl text-green-400">
      Melakukan operasi matematika dari data yang sudah dibuat :
      {{ multiply(baseValue) }}
    </h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      baseMultiply: 5,
      baseValue: 2,
    };
  },
  methods: {
    add_1() {
      return 2 + 3 + 5;
    },

    add_2(a, b, c) {
      return a + b + c;
    },

    multiply(num) {
      return num * this.baseMultiply;
    },
  },
};
</script>
