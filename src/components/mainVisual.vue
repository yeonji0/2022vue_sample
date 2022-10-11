<template>

  <swiper :navigation="true" :modules="modules" :loop="true" class="mySwiper" >
    <swiper-slide 
    v-for="(item,i) in swiperView" 
    :key="item"
    :style="{'background-color': `${swiperView[i].color}`}">
      <!-- <div :style="{'background-color':`${item.color}`}" class="innerItem"> -->
      <div class="innerItem">
        <img :src="`./img/swiper/${item.src}`" alt="">
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/navigation";


// import required modules
import { Navigation } from "swiper";

import sData from "@/data/swiper.js";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation],
      swiperView: sData,
    };
  },
};
</script>


<style lang="scss">
.mySwiper {
  .swiper-slide{
    height: 400px;
    .innerItem{
      height: 100%;
    }
    img{
      display: block;margin: 0 auto;
    }
  }
}
</style>