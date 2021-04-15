<template>
  <div id="app">
    <!-- 'using'/placing the components in the html of this component (app) -->
    <header-component />
    <body-component />
    <footer-component />
  </div>
</template>

<script>
//imported components for header, body, and footer to this page
import BodyComponent from "./components/BodyComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import HeaderComponent from "./components/HeaderComponent.vue";

//register the new components in this page so we can use it in our HTML
export default {
  //register this component for use when exporting
  name: "App",
  //register these components within this component
  components: {
    HeaderComponent,
    BodyComponent,
    FooterComponent,
  },
};
</script>

<style>
/* css for the WHOLE app */
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
</style>
