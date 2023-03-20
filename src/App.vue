<template>
  <div id="app">
    <v-main-wrapper />
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    vMainWrapper,
  },
};
import vMainWrapper from './components/v-main-wrapper';
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 30px;
  margin: 0;
}
</style>
