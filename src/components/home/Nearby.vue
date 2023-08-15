<template>
  <div class="nearby">
    <h2>附近店铺</h2>
    <div v-for="item in nearbyList" :key="item.id"
         class="nearby__item">
      <div class="nearby__img">
        <img :src="item.imgUrl" :alt="item.name">
      </div>
      <div class="nearby__content">
        <p class="nearby__name">
          {{ item.name }}
        </p>
        <p class="nearby__tags">
          <span v-for="(tag, index) in item.tags"
                :key="index" class="nearby__tagInfo">
            {{ tag }}
          </span>
        </p>
        <p class="nearby__highlight">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
f
<script setup>
  import img1 from '@/assets/images/沃尔玛.png'
  const nearbyList = [{
    id: 1,
    name: '沃尔玛',
    imgUrl: img1,
    tags: ['月销1万+', '起送￥0', '基础运费￥0'],
    description: 'VIP尊享满89元减4元运费券（每月3张）'
  },
    {
      id: 2,
      name: '沃尔玛',
      imgUrl: img1,
      tags: ['月销1万+', '起送￥0', '基础运费￥0'],
      description: 'VIP尊享满89元减4元运费券（每月3张）'
    },
    {
      id: 3,
      name: '沃尔玛',
      imgUrl: img1,
      tags: ['月销1万+', '起送￥0', '基础运费￥0'],
      description: 'VIP尊享满89元减4元运费券（每月3张）'
    }]
</script>

<style scoped lang="scss">
@import "../../style/variables";

.nearby {
  margin-top: 16px;
  color: $content-fontColor;

  &__item {
    display: flex;
    align-items: center;

    .nearby__img {
      width: 56px;
      height: 56px;
      margin-right: 16px;

      img {
        width: 100%;
      }
    }

    .nearby__content {
      flex: 1;
      border-bottom: 1px solid $content-bgColor;
      padding: 16px 0 12px 0;

      .nearby__name {
        font-size: 0.16rem;
      }

      .nearby__tags {
        margin-top: 8px;

        .nearby__tagInfo {
          font-size: 0.13rem;
          margin-right: 16px;
        }
      }

      .nearby__highlight {
        margin-top: 8px;
        font-size: 0.13rem;
        color: #E93B3B;
      }
    }
  }
}
</style>
