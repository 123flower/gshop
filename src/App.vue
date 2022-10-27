<template>
  <div class="app">
    <HeaderTop/>
    <div class="router_pages">
      <router-view/>
    </div>
    <FooterGuide v-show="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue';
import HeaderTop from './components/HeaderTop/HeaderTop.vue';
export default {
  name: 'App',
  components:{
    FooterGuide,
    HeaderTop
  }
}
</script>

<style lang="stylus">
.app
  width: 100%
  height: 100%
  background: #f5f5f5

  
</style>>
