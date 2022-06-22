<template>
  <div id="app" class="">
  
    <MyHeader class="fix-top"></MyHeader>

    <MyMain class=""></MyMain>

    <BannerDcMerch></bannerDcMerch>

    <MyFooter class="jumbotron"></MyFooter>
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';
import BannerDcMerch from './components/BannerDcMerch.vue';


export default {
  name: 'App',
  
  components: { MyHeader, MyMain, MyFooter, BannerDcMerch,
  
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  .fix-top{
    position:fixed;
    right:0;
    left:0;
    top:2rem;
    background-color:#fff;
  }
}
</style>
