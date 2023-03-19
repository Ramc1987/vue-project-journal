<template>
  <div class="v-main-wrapper">
    <p>{{ title }}</p>
    <v-header />
    <c-categories />
  </div>
</template>

<script>
import vHeader from './v-header';
import cCategories from './categories/c-categories';

export default {
  name: 'v-main-wrapper',
  components: {
    vHeader,
    cCategories,
  },
  props: {},
  data() {
    return {
      title: 'main wrapper',
    };
  },
};
</script>

<style>
.v-main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  max-width: 900px;
  margin: 0 auto;
}
</style>
