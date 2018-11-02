<template>
  <div>
      <header-componen></header-componen>
      <home-slider></home-slider>
      <novice></novice>
      <Borrow/>
      <Money/>
      <Product/>
      <Life />
      <Footer />
      <Navbar />
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import Footer from '../public/footer'
import Navbar from '../public/navbar'

import HomeSlider from './homeSlider'
import Novice from './novice'
import Borrow from './borrow'
import Money from './money'
import Product from './product'
import Life from './life'

export default {
  components: {
    HeaderComponen,
    HomeSlider,
    Novice,
    Borrow,
    Money,
    Product,
    Life,
    Footer,
    Navbar
  }
}
</script>
<style lang="scss" >
@import '../../css/reset.css'
</style>
>