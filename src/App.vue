<template>
  <q-layout view="hHh lpR fFf">
    <Navbar />
    <q-page-container>
      <q-page>
        <Carousel />
        <Cards  />
      </q-page>
    </q-page-container>
    <Footer />
  </q-layout>
</template>

<script>
import Navbar from './components/navbar.vue';
import Carousel from './components/carousel.vue';
import Cards from './components/cards.vue';
import Footer from './components/footer.vue';

export default {
  components: {
    Navbar,
    Carousel,
    Cards,
    Footer
  },
};
</script>

<style scoped>
.q-layout {
  background-color: #c78f00;
}
</style>
