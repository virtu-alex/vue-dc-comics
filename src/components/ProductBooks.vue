<template>
  <div class="product-books">
    <img :src="product.thumb" alt="product.series" />
    <h4>{{ product.series }}</h4>
  </div>
</template>

<script>
export default {
  name: "ProductBooks",
  props: {
    product: Object,
  },
};
</script>

<style lang="scss">
.product-books {
  display: flex;
  flex-wrap: wrap;
  flex-basis: calc(100% / 6);
  padding: 15px;
  img {
    height: 230px;
    min-width: 100%;
  }
}
</style>