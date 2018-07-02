<template>
  <div>
     <v-Tou></v-Tou>
     <v-state></v-state>
  </div> 
</template>
<script>
import Tou from './component/tou'
import State from './component/state'
export default {
  name: "shouye",
  components:{
   'v-Tou': Tou,
   'v-state':State
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>

</style>
