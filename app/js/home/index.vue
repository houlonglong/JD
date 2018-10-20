<template>
  <div>
      <header-componen></header-componen>
      <home-slider></home-slider>
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import HomeSlider from './homeSlider'
export default {
  components: {
    HeaderComponen,
    HomeSlider
  }
}
</script>
<style lang="scss" scoped>
@import '../../css/reset.css'
</style>
>