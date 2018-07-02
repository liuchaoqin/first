<template>
  <div>
     <v-Tou></v-Tou>
     <v-State></v-State>
     <v-Swiper></v-Swiper>
  </div> 
</template>
<script>
import Tou from './component/tou'
import State from './component/state'
import Swiper from './component/swiper'
export default {
  name: "shouye",
  components:{
   'v-Tou': Tou,
   'v-State': State,
   'v-Swiper': Swiper
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>

</style>
