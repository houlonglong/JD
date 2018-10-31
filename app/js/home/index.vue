<template>
  <div>
      <header-componen></header-componen>
      <home-slider></home-slider>
      <novice></novice>
      <Borrow/>
      <Money/>
      <Product/>
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import HomeSlider from './homeSlider'
import Novice from './novice'
import Borrow from './borrow'
import Money from './money'
import Product from './product'
export default {
  components: {
    HeaderComponen,
    HomeSlider,
    Novice,
    Borrow,
    Money,
    Product
  }
}
</script>
<style lang="scss" >
@import '../../css/reset.css'
</style>
>