vue

<template>
  <nav class="v-nav">
    <p>{{ title }}</p>
    <v-nav-list />
  </nav>
</template>

<script>
import vNavList from './v-nav-list';
export default {
  name: 'v-nav',
  components: {
    vNavList,
  },
  data() {
    return {
      title: 'Helloi',
    };
  },
};
</script>
<style></style>
