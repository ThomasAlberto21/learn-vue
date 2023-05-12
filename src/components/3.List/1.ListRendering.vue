<template>
  <!-- <div class="text-center">
    <h1
      v-for="name in names"
      :key="name"
      class="text-green-400 font-semibold text-2xl"
    >
      {{ name }}
    </h1>

    <h1
      v-for="fullName in fullNames"
      :key="id"
      class="text-green-400 font-semibold text-2xl"
    >
      {{ fullName.firstName }} {{ fullName.lastName }}
    </h1>
  </div> -->

  <div class="grid grid-flow-row grid-cols-3">
    <div
      v-for="(product, index) in products"
      :key="index"
      class="grid max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
    >
      <a href="#">
        <img class="rounded-t-lg w-96" :src="product.thumbnail" />
      </a>
      <div class="">
        <h5
          class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
        >
          {{ product.title }}
        </h5>

        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
          {{ product.description }}
        </p>

        <a
          href="#"
          class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        >
          Read more
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      names: ['Thomas', 'Frans', 'Narko', 'Teguh'],
      fullNames: [
        { id: 1, firstName: 'Thomas', lastName: 'Alberto' },
        { id: 2, firstName: 'Fransiskus', lastName: 'Berto' },
        { id: 3, firstName: 'Teguh', lastName: 'Firmansyah' },
      ],
      products: [
        {
          id: 1,
          title: 'iPhone 9',
          description: 'An apple mobile which is nothing like apple',
          price: 549,
          discountPercentage: 12.96,
          rating: 4.69,
          stock: 94,
          brand: 'Apple',
          category: 'smartphones',
          thumbnail: 'https://i.dummyjson.com/data/products/1/thumbnail.jpg',
        },
        {
          id: 2,
          title: 'iPhone X',
          description:
            'SIM-Free, Model A19211 6.5-inch Super Retina HD display with OLED technology A12 Bionic chip with ...',
          price: 899,
          discountPercentage: 17.94,
          rating: 4.44,
          stock: 34,
          brand: 'Apple',
          category: 'smartphones',
          thumbnail: 'https://i.dummyjson.com/data/products/2/thumbnail.jpg',
        },
        {
          id: 3,
          title: 'Samsung Universe 9',
          description:
            "Samsung's new variant which goes beyond Galaxy to the Universe",
          price: 1249,
          discountPercentage: 15.46,
          rating: 4.09,
          stock: 36,
          brand: 'Samsung',
          category: 'smartphones',
          thumbnail: 'https://i.dummyjson.com/data/products/3/thumbnail.jpg',
        },
      ],
    };
  },
};
</script>
