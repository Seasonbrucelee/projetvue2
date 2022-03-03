<template>
  <div class="home">
    <Carousel />
    <Jumbotron />
    <Multimedias />
    
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import Carousel from "@/components/Carousel.vue"
import Jumbotron from "@/components/Jumbotron.vue";
import Multimedias from "@/components/Multimedias.vue";

export default {
  name: 'Home',
  components: {
   // HelloWorld
    Carousel,
    Jumbotron,
    Multimedias,
  }
}
</script>
<style>  
</style>
