<template>
  <h1 class="text-green-500 text-2xl font-semibold">Hello My Name Is {{ name }}</h1>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      name: 'Thomas Alberto',
    };
  },
};
</script>
