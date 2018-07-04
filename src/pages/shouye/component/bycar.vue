<template>
  <div>
      <div class="bycar">
          <!-- 红条部分 -->
          <div class="type-top">
              <img class="bycaricon" :src="bycarimg"/>
              <p class="title">{{title}}</p>
              <p class="more">{{more}}</p>
          </div>
          <!-- 购车流程图片部分 -->
          <div class="bycar-flow">
              <div class="flow-icon" v-for="item of flowicon" :key="item.id">
                  <img class="flowimg" :src="item.imgurl"/>
              </div>    
          </div>
          <!-- 购车流程文字部分 -->
          <div class="bycar-text">
              <div class="flow-text" v-for="item of flowtext" :key="item.id">
                  <p class="flowintro">{{item.flowintro}}</p>
              </div>
          </div>
          <!-- 竖线部分 -->
          <div class="shuxian">
              <img class="xuxian" src="static/images/83-竖虚线.png"/>
          </div>
          <!-- 私人订制购车流程 -->
          <div class="siren">
              <div class="siren-icon" v-for="item of flowicon" :key="item.id">
                  <img class="flowimg" :src="item.imgurl"/>
              </div>   
          </div>

      </div>
  </div> 
</template>
<script>
export default {
  name: "bycar",
  data(){
      return{
         bycarimg:'static/images/购车流程.png',
         title:'购车流程',
         more:'更多>>',
         flowicon:[{
           id:'01',
           imgurl:'static/images/电话.png'
         },{
           id:'02',
           imgurl:'static/images/83-小虚线.png'
         },{
           id:'03',
           imgurl:'static/images/机房参观.png'
         },{
           id:'04',
           imgurl:'static/images/83-小虚线.png'
         },{
           id:'05',
           imgurl:'static/images/未选车型.png'
         },{
           id:'06',
           imgurl:'static/images/83-小虚线.png'
         },{
           id:'07',
           imgurl:'static/images/需支付定金.png'
         },{
           id:'08',
           imgurl:'static/images/83-小虚线.png'
         },{
           id:'09',
           imgurl:'static/images/入职手续办理.png'
         },{
           id:'10',
           imgurl:'static/images/83-小虚线.png'
         },{
           id:'11',
           imgurl:'static/images/提车.png'
         }],
         flowtext:[{
           id:'01',
           flowintro:'电话预约'
         },{
           id:'02',
           flowintro:'到厂参观'
         },{
           id:'03',
           flowintro:'选定车型'
         },{
           id:'04',
           flowintro:'支付定金'
         },{
           id:'05',
           flowintro:'手续办理'
         },{
           id:'06',
           flowintro:'提车回家'
         }]
         
      }  
  }
 
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.bycar
  background-color #000 
  width 100%
  padding-top .32rem
  .type-top
    width 100%
    background-color red
    line-height .54rem
    color #ffffff
    overflow hidden
    .bycaricon
      display block
      width .5rem
      height .5rem
      margin-left .32rem
      margin-top .01rem
      float left
    .title
      font-size .32rem
      float left
      line-height .54rem
      margin-left .1rem
    .more
      font-size .32rem
      float right
      margin-right .32rem 
  .bycar-flow
    width 91.5%
    margin .16rem auto 0
    display flex
    justify-content space-between
    .flow-icon
      width 9%
      .flowimg
        width .6rem
  .bycar-text
    width 98%
    margin .08rem auto 0
    display flex
    justify-content space-around
    .flow-text
      width 16.6%
      .flowintro
        width 1.14rem
        font-size .1rem
        color #fff
        text-align center
  .shuxian
    width 91.5%
    margin 0 auto 
    .xuxian
      width .6rem
      margin-left 17.3%

</style>