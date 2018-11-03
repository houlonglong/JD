<template>
  <Panel title="神券满" :class="$style.panel">
    <section :class="$style.content">
      <img src="//img12.360buyimg.com/jrpmobile/jfs/t1/7640/35/4322/21318/5bda6023E656cbbbb/b2ddefd7ef80d7aa.png?width=750&height=200" alt="">
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
        height: 200px;
        display: block;
        padding-bottom: 30px
      }
    }
  }
</style>