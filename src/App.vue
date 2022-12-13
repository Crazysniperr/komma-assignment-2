<template>
  <Nav_bar/>

</template>

<script>
import Nav_bar from './components/nav_bar.vue';
export default {
  name: 'App',
  components: {
    Nav_bar
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
