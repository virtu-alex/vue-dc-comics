<template>
  <header>
    <div class="content">
      <div class="logo">
        <img src="img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul>
          <li v-for="(link, i) in links" :key="i" :class="{active : link.current}"><a :href="link.url">{{link.text}}</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "BaseHeader",
  props: ["links"],
};
</script>

<style>

</style>