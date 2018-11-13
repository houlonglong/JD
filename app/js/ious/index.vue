<template>
  <div>
      <header-componen></header-componen>
      <Islider/>
      <Welfare/>
      <Service/>
      <Footer/>
      <Navbar/>
  </div>  
</template>

<script>
import HeaderComponen from '../public/header'
import Footer         from '../public/footer'
import Navbar         from '../public/navbar'
import Islider        from './islider.vue'
import Welfare        from './welfare.vue'
import Service        from './service.vue'
export default {
  components: {
    HeaderComponen,
    Islider,
    Welfare,
    Service,
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
