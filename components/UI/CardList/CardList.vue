<template>
  <div class="card-list py-4">
    <carousel class="" :items-to-show="1" :breakpoints="breakpoints">
      <Slide v-for="slide in 8" :key="slide">
        <UICardListCardItem />
      </Slide>

      <template #addons>
        <pagination />
      </template>
    </carousel>
  </div>
</template>
<script>
import { Carousel, Slide, Pagination } from "vue3-carousel";

export default defineComponent({
  name: "CardList",
  components: {
    Carousel,
    Slide,
    Pagination,
  },
  data: () => ({
    // Carousel breakpoints
    breakpoints: {
      1379: {
        itemsToShow: 4,
        snapAlign: "start",
        mouseDrag: true,
      },
      786: {
        itemsToShow: 2,
        snapAlign: "start",
        mouseDrag: true,
      },
    },
  }),
});
</script>
<style lang="css">
/* Carousel Style import */
@import "vue3-carousel/dist/carousel.css";

/* Carousel custom stylization */
.carousel__pagination-button.carousel__pagination-button--active::after {
  background: #08377a;
  width: 39px;
}

.carousel__pagination-button.carousel__pagination-button--active {
  width: -120px;
}

.carousel__pagination-button::after {
  background-color: #08377ab4;
  height: 8px;
}
</style>
