<template>
<div class="wrapper">
    <swiper :options="swiperOption">
      <swiper-slide v-for ="item of swiperList" :key="item.id">
        <img class="swiper-img"  :src="item.imgurl"/>
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: "shouyeswiper",
  data () {
      return {
        swiperOption: {
          pagination: '.swiper-pagination',
          loop: true
        },
        swiperList:[{
          id: '001',
          imgurl: 'static/images/2.png'
        }, {
          id:'002',
          imgurl: 'static/images/4.png'
        }]
      }
  }
  
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
   background : #fff 
.wrapper
  overflow: hidden
  width : 100%
  height :0
  padding-bottom : 55.73%
  background : #eee
  .swiper-img
      width : 100%
</style>