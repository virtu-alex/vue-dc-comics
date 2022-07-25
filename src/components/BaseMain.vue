<template>
  <main>
    <section>
      <div class="comics">
        <div class="product-books">
          <ProductBooks
            v-for="(product, i) in products"
            :key="i"
            :product="product"
          />
        </div>
      </div>
    </section>
    <section class="banner">
      <ul>
        <li v-for="(bannerInfo, i) in bannerInfos" :key="i">
          <img :src="'img/' + bannerInfo.url + '.png'" alt="" /><span>{{
            bannerInfo.text
          }}</span>
        </li>
      </ul>
    </section>
  </main>
</template>

<script>
import ProductBooks from "./ProductBooks.vue";
import json from "../../dc-comics.json";

export default {
  name: "BaseMain",
  components: {
    ProductBooks,
  },
  data() {
    return {
      products: json,
      bannerInfos: [
        {
          text: "Digital Comics",
          url: "buy-comics-digital-comics",
        },
        {
          text: "DC Merchandise",
          url: "buy-comics-merchandise",
        },
        {
          text: "Subscription",
          url: "buy-comics-subscriptions",
        },
        {
          text: "Comic Shop Locator",
          url: "buy-comics-shop-locator",
        },
        {
          text: "DC Power Visa",
          url: "buy-dc-power-visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

</style>