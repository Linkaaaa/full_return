<template>
  <div class="home">
     <TollBar></TollBar>
     <div class="home-banner">

     </div>
     <div class="home-commercial">

     </div>
     <div class="home-grid">
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>存米兑换</span>
        </div>
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>红包奖励</span>
        </div>
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>体验金计划</span>
        </div>
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>奖车计划</span>
        </div>
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>众筹计划</span>
        </div>
        <div class="grid-item">
          <img src="../../../static/images/aa.png" alt="">
          <span>发布广告</span>
        </div>
     </div>
     <div class="home-server">
       <div class="server-left">
         <p>客户服务中心</p>
         <span>您的满意是我们最大的追求</span>
       </div>
       <div>
          <img src="../../../static/images/aa.png" alt="">
       </div>
     </div>
  </div>
</template>

<script>
import TollBar from '../../components/ToolBar'
export default {
  name: 'Home',
  components:{
    TollBar
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .home{
    width: 100%;
  }

  .home-banner {
    width: 100%;
    height: 15rem;
    background: url('../../../static/images/banner.png') no-repeat;
    background-size: contain;
  }
  .home-commercial {
    width: 100%;
    height: 3.5rem;
    background-color: aqua
  }
  .home-grid {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;

  }
  .grid-item {
    width: 33.33%;
    height: 11rem;
    display: flex;
    flex-direction: column;
    font-size: 1.3rem;
    align-items: center;
    justify-content: center;
  }
  .grid-item>img {
    width: 4rem;
    height: 4rem;
  }
  .grid-item>span {
    margin-top: 1rem;
  }
  .home-server {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  .server-left {
    margin-left:3rem; 
    padding: 0.3rem 0rem;
  }
  .server-left>p{
    font-size: 1.6rem;
  }
   .server-left>span{
     display: inline-block;
    font-size: 1.2rem;
    margin-top: 0.5rem;
  }
</style>
