*/Descrizione:
Create un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.
Questo bonus nasconde un'insidia legata alla renderizzazione delle immagini che potrebbe farvi venire qualche grattacapo! Cercate di trovare una soluzione da veri programmatori e proprio in caso di emergenza, aprite un ticket!
/*

<template>
  <div id="app">
    <BaseHeader :links="links" />
    
    <BaseMain />
    <BaseFooter :links="links" />
    <LinksFooter />
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import BaseMain from "./components/BaseMain.vue";
import BaseFooter from "./components/BaseFooter.vue";
import LinksFooter from "./components/LinksFooter.vue";

export default {
  name: "App",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter,
    LinksFooter,
    
  },
};
</script>

<style lang="scss">
@import "./assets/sass/style.scss";
#app {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

body {
  background-color: black;
}

.container {
  margin: 0 auto;
}

img {
  max-width: 100%;
  height: auto;
}

h1 {
  margin: 0;
}

ul {
  list-style-type: none;
}

ul li {
  padding: 0px 10px;
}

a {
  text-decoration: none;
}
</style>
