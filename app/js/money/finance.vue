<template>
  <Panel  title="理财精选" :class="$style.panel">
    <section :class="$style.content">
      <div :class="$style.item">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t8929/33/1393593833/1749/1e115bd7/59b900e6N73c7b311.png?width=56&height=56" alt="">
        <div>
          <h4>月度理财</h4>
          <p>预期年化收益率4.5%</p>
        </div>
        <em>去赚钱 > </em>
      </div>
      <div :class="$style.item">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t8962/170/1384497943/2594/aa2a2ad9/59b9011bNf3b01bea.png?width=56&height=56" alt="">
        <div>
          <h4>季度理财</h4>
          <p>预期年化收益率4.5%</p>
        </div>
        <em>去赚钱 > </em>
      </div>
      <div :class="$style.item">
        <img src="//img12.360buyimg.com/jrpmobile/jfs/t8902/275/1411242449/2807/a2cc902a/59b90111N4e88098c.png?width=56&height=56" alt="">
        <div>
          <h4>年度理财</h4>
          <p>预期年化收益率4.5%</p>
        </div>
        <em>去赚钱 > </em>
      </div>
    </section>
  </Panel>
</template>

<script>
  import Panel from '../core/panel.vue'
  export default {
    components: {
      Panel
    }
  }
</script>

<style lang="scss" module>
  @import "../../css/element.scss";
  .panel{
    @include panel;
    >h4{
      border-bottom: 1px solid #ddd;
    }
    .content{
      @include flex;
      .item{
         @include flex(row);
         align-items: center;
         height: 140px;
         &:after{
           content: " ";
           box-sizing: border-box;
           width: 100%;
           border-bottom: 1px solid  #ddd;
           margin-left: 150px;
         }
         &:last-child:after{
           border-bottom: 1px solid  #fff;
         }
         >img{
           width: 88px;
           height: 88px;
           display: inline-block;
           margin: 0 32px;  
         }
         >div{
           font-size: 35px;
           color: #333;
           line-height: 1.3;
           width: 334px;
           p{
             color: #ff3232;
             font-size: 24px;
             white-space: nowrap;
             text-overflow: ellipsis;
             overflow: hidden;
           }
         }
         >em{
           color: #ff801a;
           font-size: 28px
         }
      }
    }
  }

</style>