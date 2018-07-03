<template>
  <div>
      <div class="about-icon">
          <img class="icon-font" :src="icon"/>
          <h1>{{title}}</h1>
          <p class="enlish">{{en}}</p>
          <div class="line"></div>
          <p class="wenzi">{{intro}}</p>
      </div>
  </div> 
</template>
<script>
export default {
  name: "about",
  data(){
      return{
          title:'关于我们',
          en:'ABOUT US',
          icon:"static/images/account.png",
          intro:"车质尚(北京)汽车制造有限公司，位于北京密云经济开发区，总占地面积超过3.6万平方米，总资产高达2亿以上，是迄今为止全球对商务车改装投入研发最大的公司，拥有世界改装行业最大的研发团队，设计研发人员多达70余人，占总团队人数的26%；公司旗下设有座椅事业部、电控事业部、模具研发事业部、精细化桃木事业部、缝纫裁剪事业部、零备件事业部、蒙皮工艺事业部、超级碳纤维事业部、总装事业部、生产中心、色彩研发中心、设计创意中心合计9个事业部3个中心其中技术工程师设计师多来自江森自控座椅团队、长城汽车设计院、清华大学等国内大型主机厂；色彩设计师是日本色彩研究会（AFT）认证配色设计师，创意设计师是英国（FGA）珠宝认证设计师。 公司秉承“至真至诚 • 至信至远”的服务理念，致力于打造世界高端商务车引领者，为客户豪华舒适、商务洽谈出行保驾护航。我们不是改装车，我们是在将美与品味融入到每一辆汽车中，让每一款产品至精至美，无可挑剔，让车质尚改装的每一辆汽车如珠宝一样闪烁璀璨，散发着独一无二的光芒，沉淀人类发展的文明。"
      }
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
.about-icon
  width: 100%
  background-color: #000
  padding-top: .38rem
  .icon-font
    display: block
    width :.46rem
    height :.46rem
    margin :0 auto
  h1
    width :100%
    font-size: .4rem
    color: #fff
    margin-top :.16rem
    text-align: center
  .enlish
    width:100% 
    font-size: .1rem
    margin-top: .1rem
    text-align: center
    color: #ffffff
  .line
    background-color:red
    width :1.6rem
    height :1px
    margin : .12rem auto
  .wenzi
    font-size :.1rem
    color :#fff
    width:90.9%
    margin :0 auto
    padding:.32rem
    line-height :.35rem
</style>