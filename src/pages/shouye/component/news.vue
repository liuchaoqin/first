<template>
  <div>
      <div class="news">
          <!-- 红条部分 -->
          <div class="type-top">
              <img class="newicon" :src="newimg"/>
              <p class="title">{{title}}</p>
              <p class="more">{{more}}</p>
          </div>
          <!-- 新闻展示部分 -->
          <ul class="type-display">
              <li class="new-img" v-for="item of newList" :key='item.id'>
                  <img class="new-type" :src="item.imgurl"/>
                  <p class="img-intro">{{item.imgintro}}<span class="details">{{item.detail}}</span></p>
              </li>
          </ul>

      </div>
  </div> 
</template>
<script>
export default {
  name: "cartype",
  data(){
      return{
         newimg:'static/images/新闻.png',
         title:'新闻',
         more:'更多>>',
         newList:[{
             id:'1',
             imgurl:'static/images/3.png',
             imgintro:'111111',
             detail:'详情>>'
         },
         {   id:'2',
             imgurl:'static/images/3.png',
             imgintro:'111111',
             detail:'详情>>'
         },{ 
             id:'3',
             imgurl:'static/images/3.png',
             imgintro:'111111',
             detail:'详情>>'
         },{
             id:'4',
             imgurl:'static/images/3.png',
             imgintro:'111111',
             detail:'详情>>'
         }]
      }  
  }
 
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.news
  background-color #000 
  width 100%
  padding-top .32rem
  .type-top
    width 100%
    background-color red
    line-height .54rem
    color #ffffff
    overflow hidden
    .newicon
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
  .type-display
    margin .32rem auto 0
    width 96%
    display flex
    justify-content space-around
    flex-wrap wrap
    .new-img
      width 48%
      height 2.8rem
      .new-type
        width 3.45rem
        height 2.32rem
      .img-intro
        font-size .1rem
        color #fff
        margin-top .01rem
        .details
          color red
          display block
          float right 
          
</style>