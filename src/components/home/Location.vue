<template>
  <div class="location">
    <local-two class="location__local" theme="outline" size="20"/>
    <span class="location__address">四川交通职业技术学院</span>
    <remind class="location__remind" theme="outline" size="20"/>
  </div>
</template>

<script setup>

import { LocalTwo, Remind } from '@icon-park/vue-next'
</script>

<style scoped lang="scss">
@import "@/style/variables";
@import "@/style/mixins";

.location {
  font-size: 0.16rem;
  margin-top: 16px;
  display: flex;
  align-items: center;
  color: $content-fontColor;

  &__local {
    margin-right: 6px;
  }

  &__address {
    flex: 1;
    @include ellipsis;
  }

  &__remind {
    margin-left: 6px;
  }
}
</style>
