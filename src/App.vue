<template>

<header-view></header-view>
<main-visual></main-visual>
<direct-banner v-bind:data="directData"></direct-banner>
<div class="container">
  <div class="row">
    <div class="col-md-6 bg-primary">test</div>
    <div class="col-md-6 bg-info">test</div>
  </div>
</div>
  
</template>

<script>
import headerView from "./components/HeaderView.vue"
import mainVisual from "./components/mainVisual.vue"
import DirectBanner from "./components/directBanner.vue"

import directs from "./data/directs.js"

export default {
  components:{
    headerView,
    mainVisual,
    DirectBanner,
  },
  data(){
    return{
      directData:directs
    }

  }

}
</script>

<style>
*{margin: 0;padding: 0;}
ul,li{list-style: none;}
a:link, a:visited{text-decoration: none; color: #333;}
.container{width: 1200px; margin: 0 auto; }

</style>