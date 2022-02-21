<template>
  <div id="app">
   <Navbar />
   <Carousel />
   <Jumbotron />
   <Footer />
   
  </div>
</template>
<script>
import Navbar from "./components/Navbar.vue";
import Carousel from "./components/Carousel.vue"
import Jumbotron from "./components/Jumbotron.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Carousel,
    Jumbotron,
    Footer, 
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
