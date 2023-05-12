<template>
  <!-- <Binding /> -->
  <!-- <Conditional /> -->
  <List />
</template>

<script>
import Binding from './views/1.Binding.vue';
import Conditional from './views/2.Conditional.vue';
import List from './views/3.List.vue';

export default {
  name: 'App',
  components: {
    Binding,
    Conditional,
    List,
  },
};
</script>
