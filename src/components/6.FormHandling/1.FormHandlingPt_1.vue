<!-- Todo -->
<!-- V-Model adalah salah satu fitur dalam Vue.js yang digunakan untuk mengaitkan data dengan elemen input, seperti input teks, checkbox, atau select box. Ini memungkinkan Anda untuk membuat dua arah binding antara data Vue.js dan elemen input, sehingga perubahan pada elemen input akan secara otomatis memperbarui data, dan sebaliknya. -->

<template>
  <div class="text-white">
    {{ JSON.stringify(formValues, null, 2) }}
  </div>

  <form action="">
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
      <label for="hobby" class="text-green-500 font-semibold text-2xl block"
        >My Hobby</label
      >
      <select
        name=""
        id="my-hobby"
        class="border border-1 border-green-400 px-5 text-white"
        v-model="formValues.hobby"
      >
        <option value="">Select Your Hobby</option>
        <option value="Berenang">Berenang</option>
        <option value="Makan">Makan</option>
        <option value="Belajar">Belajar</option>
        <option value="Olahraga">Olahraga</option>
      </select>
    </div>

    <div>
      <label for="hobby" class="text-green-500 font-semibold text-2xl block"
        >Skill</label
      >
      <!-- Multiple digunakan untuk mengizinkan pengguna memilih beberapa opsi sekaligus.  -->
      <select
        name=""
        id="skill"
        class="border border-1 border-green-400 px-5 text-white"
        multiple
        v-model="formValues.skill"
      >
        <option value="Javascript">Javascript</option>
        <option value="PHP">PHP</option>
        <option value="Python">Python</option>
        <option value="Node JS">Node JS</option>
      </select>
    </div>
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
    };
  },
};
</script>
