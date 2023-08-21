<template>
  <div class="card-list py-4">
    <carousel class="" :items-to-show="1.5">
      <Slide v-for="slide in 4" :key="slide">
        <UICardListCardItem />
      </Slide>

      <template #addons>
        <navigation />
        <pagination />
      </template>
    </carousel>
  </div>
</template>
<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
  name: "App",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
};
</script>
<style lang="css"></style>
