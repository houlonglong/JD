<template>
  <Panel title="更多服务" :class="$style.panel">
    <section :class="$style.content">
      <div :class="$style.item" v-for="item in items" :key="item.text">
        <img :src="item.img"/>
        <p>{{item.text}}</p>
      </div>
    </section>
  </Panel>
</template>

<script>
import Panel from '../core/panel';
export default {
  data() {
    return {
      items: [
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132',
          text: '小白卡'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132',
          text: '借钱'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132',
          text: '抢钢镚'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135',
          text: '白条提额'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t1/520/34/950/3686/5b9239e3Eaaf5465c/8d8c35badacfc114.png?width=90&height=90',
          text: '工资理财'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t1/1216/39/659/4516/5b923b1cE5943d1c6/dabaf8b842f57eb9.png?width=90&height=90',
          text: '众筹'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t1/3924/28/657/3552/5b9240dbE60256c31/78b52d5ab675f800.png?width=90&height=90',
          text: '租房'
        },
        {
          img: '//img12.360buyimg.com/jrpmobile/jfs/t1/479/25/929/9198/5b9243aaE826fc97b/37ef0a7cdfd24238.png?width=120&height=120',
          text: '电影票'
        }
      ]
    }
  },

  components: {
    Panel
  }
}
</script>

<style lang="scss" module>
  @import '../../css/element.scss';
  .panel {
    @include panel;
    .content {
      @include flex(row);
      .item {
        width: 160px;
        height: 144px;
        text-align: center;
        margin-bottom: 40px;
        img {
          width: 90px;
          height: 90px;
        }
        p {
          color: #666666;
          font-size: 26px;
        }
      }
    }
  }
</style>