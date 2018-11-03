<template>
  <Panel title="神券满" :class="$style.panel">
    <section :class="$style.content">
      <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/5342/12/14193/47479/5bda785aE196eaef5/eecb92594d88ba72.jpg?width=750&height=2200" alt="">
    </section>
  </Panel> 
</template>

<script>
import Panel from '../core/panel.vue'
export default {
    components:{
      Panel
    }
}
</script>

<style lang="scss" module>
  @import "../../css/element.scss";
  .panel{
    @include panel;
    >h4{
      display: none;
    }
    .content{
      img {
        width: 100%;
        height: 230px;
      }
    }
  }
</style>