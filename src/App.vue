<template>
  <Header />
  <main>
    <Hero />
    <Features />
    <Info />
    <Testimonials />
  </main>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Features from './components/Features.vue';
import Info from './components/Info.vue';
import Testimonials from './components/Testimonials.vue';

export default {
  name: 'App',
  components: { Header, Hero, Features, Info, Testimonials },
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
