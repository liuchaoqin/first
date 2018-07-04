<template>
  <div>
      <div class="type">
          <!-- 红条部分 -->
          <div class="type-top">
              <img class="car" :src="typeimg"/>
              <p class="title">{{title}}</p>
              <p class="more" v-show="!isShowAll" @click="showAll">{{more}}</p>
          </div>
          <!-- 车型展示部分 -->
          <ul class="type-display">
              <li class="car-img" v-for="(item,index) of imgList" :key='index'>
                  <img class="car-type" :src="item.imgurl"/>
                  <p class="img-intro">{{item.imgintro}}</p>
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
         typeimg:'static/images/车型.png',
         title:'车型',
         more:'更多>>',
         carList:[{
             id:'1',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },
         {   id:'2',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },{ 
             id:'3',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },{
             id:'4',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },
         { 
             id:'5',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },{
             id:'6',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },
         { 
             id:'7',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         },{
             id:'8',
             imgurl:'static/images/3.png',
             imgintro:'111111'
         }],
         isShowAll:false
      }
  },
  computed:{
      imgList(){
        if(!this.isShowAll){
            return this.carList.slice(0,4)
        }
        return this.carList;
      }
  },
  methods:{
      showAll(){
          this.isShowAll = true;
      }
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.type
  background-color #000 
  width 100%
  .type-top
    width 100%
    background-color red
    line-height .54rem
    color #ffffff
    overflow hidden
    .car
      display block
      width .5rem
      height .5rem
      margin-left .32rem
      margin-top .05rem
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
    .car-img
      width 48%
      height 2.8rem
      .car-type
        width 3.45rem
        height 2.32rem
      .img-intro
        font-size .1rem
        color #fff
        margin-top .01rem
</style>
