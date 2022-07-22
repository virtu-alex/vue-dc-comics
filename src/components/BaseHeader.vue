<template>
  <header>
    <div class="header-content">
      <div class="header-logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul>
          <li><a href="">Characters</a></li>
          <li><a href="">Comics</a></li>
          <li><a href="">Movies</a></li>
          <li><a href="">TV</a></li>
          <li><a href="">Games</a></li>
          <li><a href="">Collectibles</a></li>
          <li><a href="">Video</a></li>
          <li><a href="">Fans</a></li>
          <li><a href="">News</a></li>
          <li><a href="">Shop</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "BaseHeader",
};
</script>

<style>
header {
  color: white;
  background-color: white;
  position: fixed;
  left: 0;
  top: 0;
  right: 0;
  padding: 20px;
}

.header-logo {
    padding-right: 200px;
}

.header-content {
  display: flex;
  align-items: center;
  justify-content: center;
}

.header-content img {
  height: 80px;
  justify-self: start;
}

ul {
  list-style-type: none;
  justify-content: end;
  display: flex;
}
ul li {
  padding: 0px 10px;
}

ul li a {
  text-decoration: none;
  color: black;
}
</style>