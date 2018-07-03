<template>
  <div>
     <v-Tou></v-Tou>
     <v-State></v-State>
     <v-Swiper></v-Swiper>
     <v-About></v-About>
     <v-Cartype></v-Cartype>
     <v-News></v-News>
     <v-Bycar></v-Bycar>
  </div> 
</template>
<script>
import Tou from './component/tou'
import State from './component/state'
import Swiper from './component/swiper'
import About from './component/about'
import Cartype from './component/cartype'
import News from './component/news'
import Bycar from './component/bycar'
export default {
  name: "shouye",
  components:{
   'v-Tou': Tou,
   'v-State': State,
   'v-Swiper': Swiper,
   'v-About': About,
   'v-Cartype':Cartype,
   'v-News':News,
   'v-Bycar':Bycar
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>

</style>
