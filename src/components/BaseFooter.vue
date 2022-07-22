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
        <li><a href="#">Terms Of Use</a></li>
        <li><a href="#">Privacy policy (New)</a></li>
        <li><a href="#">Ad Choices</a></li>
        <li><a href="#">Advertising</a></li>
        <li><a href="#">Jobs</a></li>
        <li><a href="#">Subscriptions</a></li>
        <li><a href="#">Talent Workshop</a></li>
        <li><a href="#">CPSC Cerificates</a></li>
        <li><a href="#">Ratings</a></li>
        <li><a href="#">Shop Help</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
      <ul>
        <li>
          <h4>SITES</h4>
        </li>
        <li><a href="#">DC</a></li>
        <li><a href="#">MAD Magazine</a></li>
        <li><a href="#">DC Kids</a></li>
        <li><a href="#">DC Universe</a></li>
        <li><a href="#">DC Power Visa</a></li>
      </ul>
    </nav>
      <div class="dc-logo"></div>
      <div class="bottom-footer">

      </div>
  </footer>
</template>

<script>
export default {
  name: "BaseFooter",
  props: ["links"],
};
</script>

<style>
</style>