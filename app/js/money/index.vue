<template>
  <div>
      <header-componen></header-componen>
      <Mslider></Mslider>
      <AdOne />
      <Money />
      <AdTwo />
      <Finance />
      <AdThree />
      <Footer cname="mfooter"/>
      <Navbar />
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import Footer         from '../public/footer'
import Navbar         from '../public/navbar'
import Mslider        from './mslider.vue'
import AdOne          from './ad_one.vue'
import Money          from './money.vue'
import AdTwo          from './ad_two.vue'
import Finance        from './finance.vue'
import AdThree          from './ad_three.vue'
export default {
  components: {
    HeaderComponen,
    Mslider,
    AdOne,
    Money,
    AdTwo,
    Finance,
    AdThree,
    Footer,
    Navbar
  }
}
</script>
<style lang="scss" >
@import '../../css/reset.css';
  .mfooter{
    ul{
      li:first-child{
        display: none;
      }
    }
  }
</style>
