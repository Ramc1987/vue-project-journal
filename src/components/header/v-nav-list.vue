<template>
  <ul class="v-nav-list reset-list">
    <li class="v-nav-item">
      <a class="v-nav-link" href="#">Рубрики</a>
    </li>
    <li class="v-nav-item">
      <a class="v-nav-link" href="#">срочно</a>
    </li>
    <li class="v-nav-item">
      <a class="v-nav-link" href="#">АРХИВ</a>
    </li>
    <li class="v-nav-item">
      <a class="v-nav-link" href="#">La patrimoine</a>
    </li>
    <li class="v-nav-item" v-if="visible">
      <a class="v-nav-link" href="#">АЛЬМАНАХ ЭТЕРНАЛИЗМА Flipbook</a>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'v-nav-list',
  components: {},
  props: {},
  data() {
    return {
      visible: true,
    };
  },
  methods: {
    hideLastLink: function () {},
  },
};
</script>

<style lang="scss">
.v-nav-list {
  list-style-type: none;
  display: flex;
}

.v-nav-item {
  &:not(:last-child) {
    margin-right: 20px;
  }
}
</style>
