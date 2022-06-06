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
@use './styles/variables.scss' as *;

*,
*::before,
*::after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

img {
  display: block;
}

html {
  background-color: $background-main;
}
</style>
