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
      <BaseHeader />
      <BaseMain />
      <BaseFooter />
    </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import BaseMain from "./components/BaseMain.vue";
import BaseFooter from "./components/BaseFooter.vue";

export default {
  name: "App",
  components: {
    BaseHeader,
    BaseMain,
    BaseFooter
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
body {
  height: 100vh;
  background-color: black;
}
.container {
  margin: 0 auto;
  max-width: 1400px;
}
img {
  max-width: 100%;
  height: auto;
}
</style>
