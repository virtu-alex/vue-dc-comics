<template>
  <main>
    <section>
      <h1>--Content goes here--</h1>
    </section>
    <section class="banner">
      <ul>
        <li v-for="(bannerInfo, i) in bannerInfos" :key="i">
          <img :src="'img/' + bannerInfo.url + '.png'" alt="" /><span>{{
            bannerInfo.text
          }}</span>
        </li>
        <!-- <li><img src="../assets/img/buy-comics-merchandise.png" alt=""><span>DIGITAL COMICS</span></li>
        <li><img src="../assets/img/buy-comics-subscriptions.png" alt=""><span>DIGITAL COMICS</span></li>
        <li><img src="../assets/img/buy-comics-shop-locator.png" alt=""><span>DIGITAL COMICS</span></li>
        <li><img src="../assets/img/buy-dc-power-visa.svg" alt=""><span>DIGITAL COMICS</span></li> -->
       
      </ul>
    </section>
  </main>
</template>

<script>
export default {
  name: "BaseMain",
  data() {
    return {
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

<style scoped>
img {
  width: 50px;
}
</style>