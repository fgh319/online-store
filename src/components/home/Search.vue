<template>
  <div class="search">
    <search class="search__icon" theme="outline" size="18"/>
    <input class="search__text" type="text" placeholder="山姆会员商店优惠商品">
  </div></template>
<script setup>

import { Search } from '@icon-park/vue-next'
</script>

<style scoped lang="scss">
@import "@/style/variables";

.search {
  background-color: $content-bgColor;
  border-radius: 16px;
  margin-top: 16px;
  display: flex;
  align-items: center;
  color: #b7b7b7;

  &__icon {
    margin-left: 12px;
  }

  &__text {
    font-size: 0.14rem;
    border-style: none;
    background-color: transparent;
    flex: 1;
    line-height: 32px;
    padding: 0 6px;
  }

  &__text:focus {
    outline-style: none;
  }

  &__text::placeholder {
    color: #b7b7b7;
  }
}
</style>
