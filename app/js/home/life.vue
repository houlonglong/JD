<template>
  <Panel title="生活服务" :class="$style.panel">
    <ul :class="$style.content">
      <li :class="$style.item"  v-for="item in items" :key="item.href">
        <img :src="item.src" alt="">
        <p>{{item.title}}</p>
        <p>{{item.tip}}</p>
      </li>
    </ul>
  </Panel>
</template>

<script>
import Panel from '../core/panel.vue'
export default {
  data(){
    return{
        items:[{
            src:'//img12.360buyimg.com/jrpmobile/jfs/t4375/104/1184122472/3976/89741da4/58be8a6eNf10193d0.png?width=135&height=135',
            href:'//jrappgw.jd.com/resources/downloadApp.html?id=188&activityid=252&sid=',
            title:'惠加油'
        },{
            src:'//img12.360buyimg.com/jrpmobile/jfs/t4747/185/1901740991/5892/1383fb93/58f57851N17ee6993.jpg?width=132&height=132',
            href:'//jrappgw.jd.com/resources/downloadApp.html?id=201&activityid=253&sid=',
            title:'小白信用',
            tip:'全部升级'
        },{
            src:'//img12.360buyimg.com/jrpmobile/jfs/t3241/234/8044685271/3713/7b29f77f/58be89c8Nb9d41295.png?width=135&height=135',
            href:'//jrappgw.jd.com/resources/downloadApp.html?id=237&activityid=254&sid=',
            title:'信用卡'
        },{
            src:'//img12.360buyimg.com/jrpmobile/jfs/t3172/259/7993557249/4351/fd082707/58be8a81Nd7716a06.png?width=135&height=135',
            href:'//jrappgw.jd.com/resources/downloadApp.html?id=297&activityid=255&sid=',
            title:'卡转让'
        },{
            src:'//img12.360buyimg.com/jrpmobile/jfs/t3085/320/8107659086/4344/cdbba2dd/58be8acfNdadcaf00.png?width=135&height=135',
            href:'//jrappgw.jd.com/resources/downloadApp.html?id=214&activityid=256&sid=',
            title:'定期还款'
        }]
    }
  },
  components:{
    Panel
  }
}
</script>
<style lang="scss" module>
 @import "../../css/element.scss";
 .panel{
   @include panel;
   .content{
     @include flex(row);
     box-sizing: border-box;
     padding-bottom: 40px;
     .item{
       width: 20%;
       text-align: center;
       img{
         width: 90px;
         height: 90px;
       }
       p{
         font-size: 26px;
         color:#666;
         text-overflow: ellipsis;
         white-space: nowrap;
         overflow: hidden;
         margin-top: 12px;
         &:nth-child(3){
           color:#FF801A;
         }
       }
     }
   }
 }
</style>
>