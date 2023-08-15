<template>
  <div class="wrapper">
    <img src="@/assets/images/user.png" alt="avatar">
    <div class="wrapper__input">
      <input type="text" placeholder="请输入手机号">
    </div>
    <div class="wrapper__input">
      <input type="password" placeholder="请输入密码">
    </div>
    <div class="wrapper__button">登录</div>
    <div class="wrapper__registerNow">立即注册</div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
@import "@/style/variables";
  .wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100dvh;
    padding: 0 40px;
    color: $content-fontColor;
    img {
      width: 66px;
      height: 66px;
      margin-bottom: 24px;
    }
    &__input {
      width: 100%;
      margin-top: 16px;
      input {
        width: 100%;
        line-height: 48px;
        border: 1px solid #ddd;
        border-radius: 6px;
        //outline: 1px solid #0091FF;
        background: #f9f9f9;
        font-size: 0.16rem;
        padding: 0 16px;
      }
      input:focus {
        outline: 2px solid #0091FF;
      }
    }
    &__button {
      width: 100%;
      margin-top: 32px;
      height: 48px;
      background-color: #0091FF;
      box-shadow: 0 4px 8px 0 rgba(0,145,255,0.32);
      border-radius: 4px;
      color: #fff;
      font-size: 0.16rem;
      line-height: 48px;
      text-align: center;
      letter-spacing: 8px;
      text-indent: 8px;
    }
    &__registerNow {
      width: 100%;
      margin-top: 16px;
      font-size: 0.14rem;
      color: #777;
      text-align: center;
    }
  }
</style>
