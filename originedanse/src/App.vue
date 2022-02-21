<template>
  <div id="app">
   <Navbar />
   <Carousel />
   <Jumbotron />
   <Multimedias />
   <Footer />
   <Icones />
   
  </div>
</template>
<script>
import Navbar from "./components/Navbar.vue";
import Carousel from "./components/Carousel.vue"
import Jumbotron from "./components/Jumbotron.vue";
import Multimedias from "./components/Multimedias.vue";
import Footer from "./components/Footer.vue";
import Icones from "./components/Icones.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Carousel,
    Jumbotron,
    Multimedias,
    Footer, 
    Icones,
  }
};
</script>
<style>
#app {
  font-family:'Ubuntu', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color:  #031472;
  color:#b4351c;
  font-size: 30px;
}
</style>
