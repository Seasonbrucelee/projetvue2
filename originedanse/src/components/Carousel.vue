<template>
  <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <!-- <div class="carousel-item active">
        <img src="@/assets/eyezmiho.jpg" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="@/assets/wrestlerillest.jpg" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="@/assets/nach-krump-2.jpg" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="@/assets/img-7645.jpg" class="d-block w-100" alt="...">
      </div> -->
      <Slides v-for="(slide,index) in slides" :key="index" :id="slide.id" :image="slide.image"  />
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script>
import Slides from '@/components/Slides.vue'
import axios from 'axios'

export default {
  name: 'Carousel',
  components: {
    Slides,
    },
    // data(){
    //     return {
    //         slides:[
    //             {
    //                 id:1,
    //                 image:'eyezmiho.jpg',
    //             },
    //             {
    //                 id:2,
    //                 image:'wrestlerillest.jpg',
    //             },
    //             {
    //                 id:3,
    //                 image:'nach-krump-2.jpg',
    //             },
    //             {
    //                 id:4,
    //                 image:'img-7645.jpg',
    //             }
    //         ],
    //     }
    // },
  data(){
    return {
        slides:[],
        errors: []
    }
  },
    // Fetches Details when the component is created.
  created() {
    axios.get(`http://localhost:8080/slides.json`)
    .then(response => {
      // JSON responses are automatically parsed.
      this.slides = response.data.slides
    })
    .catch(e => {
      this.errors.push(e)
    })
  }  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
