<template>
  <div>
      <header-componen></header-componen>
      <home-slider></home-slider>
      <novice>111111</novice>
      
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import HomeSlider from './homeSlider'
import Novice from './novice'
console.log(Novice,111)
export default {
  components: {
    HeaderComponen,
    HomeSlider,
    Novice
  }
}
</script>
<style lang="scss" scoped>
@import '../../css/reset.css'
</style>
>