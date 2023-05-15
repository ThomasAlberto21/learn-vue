<template>
  <div class="text-center">
    <!-- Merubah nama sesuai button yang di click -->
    <div class="border bottom-1 border-green-500">
      <h1 class="text-2xl text-green-500 font-semibold">{{ name }}</h1>
      <button
        v-on:click="name = 'Fransiskus Berto'"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Fransiskus Berto
      </button>
      <button
        v-on:click="name = 'Teguh Firmansyah'"
        class="px-3 py-2 bg-green-500 rounded-lg"
      >
        Teguh Firmansyah
      </button>
    </div>

    <!-- Increment dan Decrement tanpa menggunakan methods -->
    <div class="border bottom-1 border-green-500">
      <h1 class="text-2xl text-green-500 font-semibold">{{ count }}</h1>
      <button
        v-on:click="count += 1"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Increment
      </button>
      <button v-on:click="count -= 1" class="px-3 py-2 bg-green-500 rounded-lg">
        Decrement
      </button>
    </div>

    <!-- Increment dan Decrement menggunakan methods -->
    <div class="border bottom-1 border-green-500">
      <h1 class="text-2xl text-green-500 font-semibold">{{ count }}</h1>
      <button
        v-on:click="increment(1)"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Increment + 1
      </button>
      <button
        v-on:click="increment(5)"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Increment + 5
      </button>
      <button
        v-on:click="decrement(1)"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Decrement - 1
      </button>
      <button
        v-on:click="decrement(5)"
        class="px-3 py-2 bg-green-500 rounded-lg mx-2"
      >
        Decrement -5
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Thomas Alberto',
      count: 0,
    };
  },
  methods: {
    increment(num) {
      this.count += num;
    },
    decrement(num) {
      this.count -= num;
    },
  },
};
</script>
