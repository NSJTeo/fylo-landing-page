<template>
  <Header />
  <main><Hero /></main>
</template>

<script>
import Header from './components/Header';
import Hero from './components/Hero';

export default {
  name: 'App',
  components: { Header, Hero },
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
