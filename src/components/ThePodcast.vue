
<template>
  <Carousel :settings='settings' :breakpoints='breakpoints'>
    <Slide v-for='(slide, index) in this.$store.state.podcastRow' :key='index'>
      <div class='carousel__item '>
      
   <a href="http://localhost:8080/" target="_blank">
      <img :src="slide" class="img-fluid " alt="">
   </a>
        
       </div>
    </Slide>

    <template #addons>
      <Pagination />
      <Navigation />
    </template>
  </Carousel>
</template>

<script>
import { defineComponent } from 'vue';
import { Carousel, Navigation, Slide, Pagination } from 'vue3-carousel';

export default defineComponent({
  name: 'ExamplePagination',
  components: {
    Pagination,
    Carousel,
    Slide,
    Navigation,
  },
  data: () => ({
    // carousel settings
    settings: {
      itemsToShow: 1,
      snapAlign: 'center',
    },
    // breakpoints are mobile first
    // any settings not specified will fallback to the carousel settings
    breakpoints: {
      // 700px and up
      700: {
        itemsToShow: 3.5,
        snapAlign: 'center',
      },
      // 1024 and up
      1024: {
        itemsToShow: 5,
        snapAlign: 'start',
      },
    },
  }),
});
</script>


<style scoped>
.carousel__item {
  min-height: 200px;
  width: 100%;

  color: var(--carousel-color-white);
  font-size: 50px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.carousel__pagination-button{

  background-color: green;

}
.carousel__slide {
  padding: 10px;
}

.carousel__prev,
.carousel__next {
  background-color: green;
  box-sizing: content-box;
  border: 5px solid white;
}
</style>