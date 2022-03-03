<template>
    <div v-if="id === 1" class="carousel-item active">
        <img :src="require(`@/assets/${image}`)" class="d-block w-100" alt="...">
    </div>
    <div v-else class="carousel-item">
        <img :src="require(`@/assets/${image}`)" class="d-block w-100" alt="...">
    </div>
</template>

<script>
export default {
  name: 'Slides',
  props: {
    id: Number,
    image:String,
  }
}
</script>