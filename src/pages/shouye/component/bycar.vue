<template>
  <div>
      <div class="bycar">
          <!-- 红条部分 -->
          <div class="type-top">
              <img class="bycaricon" :src="bycarimg"/>
              <p class="title">{{title}}</p>
              <p class="more">{{more}}</p>
          </div>
          <!-- 购车流程部分 -->
          <div class="bycar-icon">

          </div>

      </div>
  </div> 
</template>
<script>
export default {
  name: "cartype",
  data(){
      return{
         bycarimg:'static/images/购车流程.png',
         title:'购车流程',
         more:'更多>>'
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
          
</style>