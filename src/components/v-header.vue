<template>
  <header class="v-header">
    <p>{{ title }}</p>
    <v-nav />
  </header>
</template>

<script>
import vNav from './v-nav';

export default {
  name: 'v-header',
  props: {},
  components: {
    vNav,
  },
  data() {
    return {
      title: 'hello world',
    };
  },
};
</script>
<style lang="scss">
.v-header {
  width: 100%;
  background-color: tomato;
}
</style>
