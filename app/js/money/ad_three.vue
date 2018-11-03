<template>
  <Panel title="京东" :class="$style.panel">
    <section :class="$style.content">
      <img src="//img12.360buyimg.com/jrpmobile/jfs/t25603/15/1053175366/15557/ab0e663d/5b874874N4c490fc5.png?width=750&height=200" alt="">
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
    margin-bottom: 0;
    >h4{
      display: none;
    }
    .content{
      img {
        width: 100%;
        height: 200px;
        padding-bottom: 30px
      }
    }
  }
</style>