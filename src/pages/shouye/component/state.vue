<template>
  <div>
      <div class="nav">
          <div class="nav-left">
            <span class="iconfont" @click="handelClick">&#xe639;</span>
          </div>
          <div class="nav-logo">
            <img class="logo" src="static\images\车质尚LOGO@2x.png"/>
          </div>
          <div class="nav-right">
            <span class="iconfont">&#xe619;</span>
          </div>
      </div>   
  </div> 
</template>
<script>
export default {
  name: "state",
  methods:{
       handelClick () {
          
       }
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.nav
  height :.88rem
  line-height :.88rem
  color :#fff
  background-color :black
  display :flex
  justify-content :center
  .nav-left 
    width : 1.1rem
    .iconfont
      display : block
      text-align: center
  .nav-logo
    width :5.3rem
    .logo
      width :2.62rem
      height :.42rem
      display: block
      margin-left :1.34rem
      margin-top :.23rem
  .nav-right 
    width : 1.1rem
    .iconfont
      display : block
      text-align: center
</style>