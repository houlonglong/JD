<template>
  <Panel title="每日福利" :class="$style.panel">
    <section :class="$style.content">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t3298/196/6130416421/33755/a0536d3e/589bd5d4Nf32e7adc.jpg?width=374&height=160" alt="">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t3298/196/6130416421/33755/a0536d3e/589bd5d4Nf32e7adc.jpg?width=374&height=160" alt="">
        <p>不抢白不抢</p>
    </section>
  </Panel>
</template>

<script>
import Panel from '../core/panel'
export default {
  components: {
    Panel
  }
}
</script>

<style lang="scss" module>
  @import "../../css/element.scss";
  .panel {
    @include panel;
    .content {
      position: relative;
      @include flex(row);
      padding-bottom: 40px;
      img {
        width: 320px;
        height: 136px;
      }
      p {
        position: absolute;
        color: #999;
        font-size: 28px;
        right: 20px;
        top: -120px;
        height: 112px;
        line-height: 112px;
      }
    }
  }

</style>