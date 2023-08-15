<template>
  <swiper class="banner"
          :slides-per-view="1"
          :pagination="{ clickable: true }"
          :modules="modules"
          :space-between="8"
          :loop="true"
          :autoplay="{ delay: 2500, disableOnInteraction: false}"
          :speed="1000"
  >
    <swiper-slide><img class="banner__img" src="@/assets/images/banner.jpg" alt="banner"></swiper-slide>
    <swiper-slide><img class="banner__img" src="@/assets/images/banner2.jpg" alt="banner2"></swiper-slide>
    <swiper-slide><img class="banner__img" src="@/assets/images/banner3.jpg" alt="banner3"></swiper-slide>
  </swiper>
</template>

<script setup>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue'
// import Swiper core and required modules
import { Pagination, Autoplay, EffectFade } from 'swiper/modules'
// Import Swiper styles
import 'swiper/scss'
import 'swiper/scss/navigation'
import 'swiper/scss/pagination'
import 'swiper/scss/autoplay'
import 'swiper/scss/effect-fade'

const modules = [Pagination, Autoplay, EffectFade]
</script>

<style scoped lang="scss">
.banner {
  margin-top: 12px;
  aspect-ratio: 4/1;
  border-radius: 8px;

  &__img {
    width: 100%;
    //transform: scale(1.02);
    //transform-origin: center center;
  }
}
</style>


