<template>
  <div>
      <div class="nav">
          <div class="nav-left">
            <span class="iconfont" @click="handleclick">&#xe639;</span>
            <ul class="nav-list" v-if="show">
              <li>首页</li>
              <li>关于我们</li>
              <li>十大优势</li>
              <li>车主专享</li>
              <li>匠心订制</li>
            </ul>
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
  data(){
    return{
      show: false
    }
    
  },
  methods:{
    handleclick(){
      this.show=true;
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
    .nav-list
      position :absolute
      left :0
      top:1.28rem
      width :1.7rem
      height :2rem
      background-color :#fff
      z-index :9
      li
        height :.39rem
        line-height :.39rem
        border-bottom :0.01rem solid gray
        color :gray
        font-size :.14rem 
        text-align :center
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