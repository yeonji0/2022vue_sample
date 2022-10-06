<template>

<header-view></header-view>
<main-visual></main-visual>
  
</template>

<script>
import headerView from "./components/HeaderView.vue"
import mainVisual from "./components/mainVisual.vue"
export default {
  components:{
    headerView,
    mainVisual
  }

}
</script>

<style>
*{margin: 0;padding: 0;}
ul,li{list-style: none;}
a:link, a:visited{text-decoration: none; color: #333;}
</style>