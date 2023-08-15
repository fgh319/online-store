<template>
  <div class="docker">
    <div class="docker__item docker__item--active">
      <home theme="outline" size="22"/>
      <span class="docker__title">首页</span>
    </div>
    <div class="docker__item">
      <shopping theme="outline" size="22"/>
      <span class="docker__title">购物车</span>
    </div>
    <div class="docker__item">
      <transaction-order theme="outline" size="22"/>
      <span class="docker__title">订单</span>
    </div>
    <div class="docker__item">
      <avatar theme="outline" size="22"/>
      <span class="docker__title">我的</span>
    </div>
  </div>
</template>

<script setup>
import { Avatar, Shopping, TransactionOrder, Home } from '@icon-park/vue-next'
</script>

<style scoped lang="scss">
@import "../style/variables";

.docker {
  position: absolute;
  left: 0;
  bottom: 0;
  right: 0;
  height: 50px;
  border-top: 1px solid $content-bgColor;
  display: flex;
  align-items: center;
  color: $content-fontColor;

  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    flex: 1;

    &--active {
      color: #1d9bee;
    }
  }

  &__title {
    margin-top: 2px;
  }
}
</style>
