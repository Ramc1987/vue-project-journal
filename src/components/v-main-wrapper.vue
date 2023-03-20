<template>
  <div class="v-main-wrapper">
    <div class="container">
      <v-header />
      <c-categories />
    </div>
  </div>
</template>

<script>
import vHeader from './header/v-header';
import cCategories from './categories/c-categories';

export default {
  name: 'v-main-wrapper',
  components: {
    vHeader,
    cCategories,
  },
  props: {},
  data() {
    return {};
  },
};
</script>

<style>
.v-main-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 0 auto;
}
</style>
