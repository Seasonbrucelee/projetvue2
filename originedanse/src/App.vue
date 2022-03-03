<template>
  <div id="app">
   <Navbar />

   <router-view/>
   
   <Footer />
   <Icones />
   
  </div>
</template>
<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
import Icones from "./components/Icones.vue";

export default {
  name: "App",
  components: {
    Navbar,
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
  font-size: 40px;
}
p{
  color: #0c49df;
  font-size: 30px
};
</style>
