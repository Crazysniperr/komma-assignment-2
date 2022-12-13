<template>
  <Nav_bar/>
  <Hero/>

</template>

<script>
import Nav_bar from './components/nav_bar.vue';
import Hero from './components/hero.vue';
export default {
  name: 'App',
  components: {
    Nav_bar,
    Hero
  }
}
</script>

<style>
  body {
    margin: 0;
    box-sizing: border-box;
    padding: 0;
    background-color: rgb(52,52,52);
  }
</style>
