<template>
  <div class="icons">
    <div class="icons__item" v-for="item in iconList" :key="item.id">
      <img class="icons__img" :src='item.imgUrl' :alt="item.description">
      <p class="icons__description">{{item.description}}</p>
    </div>
  </div>
</template>

<script setup>
// 导入icons图片
import img1 from '@/assets/images/超市.png'
import img2 from '@/assets/images/菜场.png'
import img3 from '@/assets/images/水果.png'
import img4 from '@/assets/images/鲜花.png'
import img5 from '@/assets/images/医药.png'
import img6 from '@/assets/images/家居.png'
import img7 from '@/assets/images/蛋糕.png'
import img8 from '@/assets/images/签到.png'
import img9 from '@/assets/images/大牌.png'
import img10 from '@/assets/images/红包.png'

const iconList =[
  {
    id: 1,
    description: '超市便利',
    imgUrl: img1
  },
  {
    id: 2,
    description: '菜市场',
    imgUrl: img2
  },
  {
    id: 3,
    description: '水果店',
    imgUrl: img3
  },
  {
    id: 4,
    description: '鲜花绿植',
    imgUrl: img4
  },
  {
    id: 5,
    description: '医药健康',
    imgUrl: img5
  },
  {
    id: 6,
    description: '家居时尚',
    imgUrl: img6
  },
  {
    id: 7,
    description: '烘焙蛋糕',
    imgUrl: img7
  },
  {
    id: 8,
    description: '签到',
    imgUrl: img8
  },
  {
    id: 9,
    description: '大牌免运',
    imgUrl: img9
  },
  {
    id: 10,
    description: '红包套餐',
    imgUrl: img10
  }
]
</script>

<style scoped lang="scss">
@import "@/style/variables";
.icons {
  display: flex;
  flex-wrap: wrap;
  margin-top: 16px;

  &__item {
    width: 20%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  &__img {
    width: 40px;
    height: 40px;
  }

  &__description {
    color: $content-fontColor;
    margin-top: 6px;
    margin-bottom: 16px;
  }
}
</style>
