<template>
  <div id="app">
    <header-component />
    <body-component />
    <footer-component />
  </div>
</template>

<script>
//put comments here
import BodyComponent from "./components/BodyComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import HeaderComponent from "./components/HeaderComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    BodyComponent,
    FooterComponent,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}
img {
  width: 300px;
}
/* body {
  display: grid;
  place-items: center;
} */
</style>
