<template>
  <section :class="cname">
    <swiper 
    :options="options" :not-next-tick="options.notNextTick">
      <swiper-slide 
      v-for="item in items"
      :key="item.id">
        <router-link :to="{name: item.href }">
          <img :src="item.src" alt="">
        </router-link>
      </swiper-slide>
      <div class="swiper-pagination" v-if="options.pagination"></div> 
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
    },
    items: {
      type: Array,
      default(){
        return []
      }
    }
  },
  comments: {
    swiper,
    swiperSlider
  }
}
</script>
<style lang="scss">
  @import "~swiper/dist/css/swiper.css";
</style>

