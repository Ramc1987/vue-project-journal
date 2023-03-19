<template>
  <header class="v-header">
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
    return {};
  },
};
</script>
<style>
.v-header {
  width: 100%;
  background-color: tomato;
}
</style>
