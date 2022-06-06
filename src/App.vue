<template>
  <Header />
</template>

<script>
import Header from './components/Header.vue';
export default {
  name: 'App',
  components: { Header },
};
</script>

<style lang="scss">
$background-main: hsl(218, 28%, 13%);
$background-secondary: hsl(217, 28%, 15%);
$background-footer: hsl(216, 53%, 9%);
</style>
