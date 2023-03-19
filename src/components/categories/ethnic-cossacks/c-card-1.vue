<template>
  <div class="c-card-1">
    <img :src="imgLink" alt="" />
    <h2 class="c-card-1__title">{{ product_data.name }}</h2>
    <p class="c-card-1__description">{{ product_data.description }}</p>
    <button class="c-card-1__ button btn">читать далее</button>
  </div>
</template>

<script>
export default {
  name: 'c-card-1',
  components: {},
  props: {
    product_data: {
      type: Object,
      default() {
        return {};
      },
    },
  },
  data() {
    return {};
  },
  computed: {
    imgLink: function () {
      const fileName = this.product_data.image;
      return require(`../../../assets/img/${fileName}`);
    },
  },
};
</script>

<style>
.c-card-1 {
  width: 200px;
  height: auto;
  background-color: rgb(227, 216, 216);
  box-shadow: 0 1px 2px #000000;
}
</style>
