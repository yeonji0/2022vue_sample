<template>
  <div class="visual">
    <swiper>
      <SwiperSlide class="item">text1</SwiperSlide>
      <SwiperSlide class="item">text2</SwiperSlide>
      <SwiperSlide class="item">text3</SwiperSlide>
      <SwiperSlide class="item">text4</SwiperSlide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>

<style lang="scss">
.visual {
  background: pink;
  margin-bottom: 20px;
  .item {
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>