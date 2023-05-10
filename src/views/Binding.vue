<!-- Todo -->
<!-- Binding di Vue.js merujuk pada cara untuk menghubungkan atau mengikat data dari objek Vue ke elemen HTML. Dengan binding, perubahan yang dilakukan pada data di dalam objek Vue akan secara otomatis memperbarui tampilan di dalam elemen HTML yang terkait. -->

<template>
  <!-- <BindingText /> -->
  <BindingHtml />
</template>

<script>
import BindingText from '../components/1.Binding/1.BindingText.vue';
import BindingHtml from '../components/1.Binding/2.BindingHtml.vue';


export default {
  components: {
    BindingText,
    BindingHtml
  },
};
</script>
