<template>
  <div class="text-white">
    <h1>{{ JSON.stringify(formValues, product, null, 2) }}</h1>
  </div>

  <form @submit="submitForm">
    <div>
      <label for="nim" class="text-green-500 font-semibold text-2xl block"
        >Nim</label
      >
      <input
        type="number"
        id="nim"
        v-model="formValues.nim"
        class="border border-1 border-green-400 px-5 text-white"
      />
    </div>

    <div>
      <label for="name" class="text-green-500 font-semibold text-2xl block"
        >Name</label
      >
      <input
        type="text"
        id="name"
        v-model="formValues.name"
        class="border border-1 border-green-400 px-5 text-white"
      />
    </div>

    <div>
      <label for="class" class="text-green-500 font-semibold text-2xl block"
        >Class</label
      >
      <input
        type="text"
        id="class"
        v-model="formValues.class"
        class="border border-1 border-green-400 px-5 text-white"
      />
    </div>

    <div>
      <label for="tidak_pedas">Tidak Pedas</label>
      <input
        type="checkbox"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.rasa"
        true-value="Tidak Pedas"
        false-value=""
      />
      <label for="tidak_pedas">Pedas</label>
      <input
        type="checkbox"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.rasa"
        true-value=" Pedas"
        false-value=""
      />
      <label for="tidak_pedas">Sangat Pedas</label>
      <input
        type="checkbox"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.rasa"
        true-value="Sangat Pedas"
        false-value=""
      />
    </div>

    <div>
      <label for="tidak_pedas">Manis</label>
      <input
        type="radio"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.manis"
        value="Manis"
      />
      <label for="tidak_pedas">Sedang</label>
      <input
        type="radio"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.manis"
        value="Sedang"
      />
      <label for="tidak_pedas">Sangat Manis</label>
      <input
        type="radio"
        name="tidak_pedas"
        id="tidak_pedas"
        v-model="product.manis"
        value="Sangat Manis"
      />
    </div>
    <button class="px-5 py-2 bg-green-400 rounded-lg text-white">Submit</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      formValues: {
        nim: '',
        name: '',
        class: '',
        hobby: '',
        skill: [],
      },
      product: {
        rasa: '',
        manis: '',
      },
    };
  },

  methods: {
    submitForm(e) {
      e.preventDefault();
      console.log('Form', this.formValues, this.product);
    },
  },
};
</script>
