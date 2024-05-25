<template>
  <q-carousel
    swipeable
    animated
    v-model="slide"
    :autoplay="autoplay"
    ref="carousel"
    infinite
  >
    <q-carousel-slide :name="1" img-src="../assets/slide1.webp" class="carousel-image"/>
    <q-carousel-slide :name="2" img-src="../assets/slide2.jpg" class="carousel-image"/>
    <q-carousel-slide :name="3" img-src="../assets/slide3.jpg" class="carousel-image"/>
    <q-carousel-slide :name="4" img-src="../assets/slide4.jpeg" class="carousel-image"/>
  </q-carousel>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      autoplay: true
    };
  }
};
</script>

<style scoped>
.carousel-image {
  width: auto;
  height: auto;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
