<template>
  <div id="app">
    <app-header></app-header>
    <PageContent></PageContent>
    <app-footer></app-footer>
    <counter></counter>
  </div>
</template>

<script>
//Registering components Locally
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import PageContent from "./components/PageContent.vue";
import Counter from "./components/Counter.vue";
export default {
  name: "App",
  components: {
    //Registering with a name
    "app-header": Header,
    "app-footer": Footer,
    counter: Counter,
    //Registering without a name
    PageContent
  }
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
