<template>
  <!-- <Binding /> -->
  <!-- <Conditional /> -->
  <!-- <List /> -->
  <!-- <Method /> -->
  <!-- <EventHandling /> -->
  <FormHandling />
</template>

<script>
import Binding from './views/1.Binding.vue';
import Conditional from './views/2.Conditional.vue';
import List from './views/3.List.vue';
import Method from './views/4.Method.vue';
import EventHandling from './views/5.EventHandling.vue';
import FormHandling from './views/6.FormHandling.vue';

export default {
  name: 'App',
  components: {
    Binding,
    Conditional,
    List,
    Method,
    EventHandling,
    FormHandling,
  },
};
</script>
