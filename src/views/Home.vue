<template>
  <div class="wrapper">
    <Location />
    <Search />
    <Banner />
    <Icons />
    <div class="gap"></div>
    <Nearby />
  </div>
  <Docker />
</template>

<script setup>
import Nearby from '@/components/home/Nearby.vue'
import Docker from '@/components/Docker.vue'
import Location from '@/components/home/Location.vue'
import Search from '@/components/home/Search.vue'
import Banner from '@/components/home/Banner.vue'
import Icons from '@/components/home/Icons.vue'
</script>

<style scoped lang="scss">
@import "@/style/variables";
  .wrapper {
    position: absolute;
    left: 0;
    top: 0;
    right: 0;
    bottom: 50px;
    padding: 0 18px 9px 18px;
    overflow-y: auto;

    .gap {
      height: 10px;
      background-color: $content-bgColor;
      margin: 0 -18px;
    }
  }
</style>
