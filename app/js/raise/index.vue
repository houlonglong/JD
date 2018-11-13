<template>
  <div>
      <header-componen></header-componen>
      <Rslider/>
      <Daily/>
      <In/>
      <More/>
      <Footer cname="mfooter"/>
      <Navbar/>
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import Footer         from '../public/footer'
import Navbar         from '../public/navbar'

import Rslider        from './rslider.vue'
import Daily        from './daily.vue'
import In        from './in.vue'
import More        from './more.vue'
export default {
  components: {
    HeaderComponen,
    Rslider,
    Daily,
    In,
    More,
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
