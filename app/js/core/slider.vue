<template>
  <section :class="cname">
    <swiper :options="options">
      <swiper-slide></swiper-slide>
    </swiper>
  </section>
</template>

<script>
import {swiper, swiperSlider} from 'vue-awesome-swiper';
export default {
  props: {
    options: {
      type: Object,
      default() {
        return {
          autoplay: '',
          loop: true,
          pagination: {
            el: '.swper-paintation'
          },
          notNextTick: false  
        }
      }
    }
  },
  comments: {
    swiper,
    swiperSlider
  }
}
</script>
<style lang="css">
  @import "~swiper/dist/css/swiper.css";
</style>

