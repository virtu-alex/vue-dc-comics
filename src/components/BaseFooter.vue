<template>
  <footer>
    <nav>
      <ul>
        <li>
          <h4>DC COMIC</h4>
        </li>
        <li v-for="(link, i) in links" :key="i">
          <a :href="link.url">{{ link.text }}</a>
        </li>
        <ul>
          <li>
            <h4>SHOP</h4>
          </li>
          <li><a href="">Shop DC</a></li>
          <li><a href="">Shop DC Collectibles</a></li>
        </ul>
      </ul>
      <ul>
        <li>
          <h4>DC</h4>
        </li>
        <li v-for="(listDc, i) in listsDc" :key="i">
          <a href="#">{{ listDc.text }}</a>
        </li>
      </ul>
      <ul>
        <li>
          <h4>SITES</h4>
        </li>
        <li v-for="(site,i) in sites" :key="i"><a href="#">{{site.text}}</a></li>
      </ul>
    </nav>
    <div class="dc-logo"></div>
  </footer>
</template>

<script>
export default {
  name: "BaseFooter",
  props: ["links"],
  data() {
    return {
      listsDc: [
        {
          text: "Terms of Use",
        },
        {
          text: "Privacy policy (new)",
        },
        {
          text: "Ad Choices",
        },
        {
          text: "Advertising",
        },
        {
          text: "Jobs",
        },
        {
          text: "Subsriptions",
        },
        {
          text: "Talent Workshop",
        },
        {
          text: "CPSC Certificates",
        },
        {
          text: "Ratings",
        },
        {
          text: "Shop Help",
        },
        {
          text: "Contact Us",
        },
      ],
      sites: [
        {
          text: "DC",
        },
        {
          text: "MAD Magazines",
        },
        {
          text: "DC Kids",
        },
        {
          text: "DC Universe",
        },
        {
          text: "DC Power visa",
        },
      ],
    };
  },
};
</script>

<style>
</style>