<template>
  <Hero/>

</template>

<script>
import Hero from './components/hero.vue';
export default {
  name: 'App',
  components: {
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
