<template>
  <div class="user_info">
    <img v-if="userInfo.img" :src="userInfo.img" alt="" class="user_img" />
    <div class="user_name">
      {{ userInfo.name }}
    </div>
    <p class="start">此处应该有自我介绍</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userInfo: {
        name: "lintong",
        age: 30,
        img: "/static/images/user.png",
      },
    };
  },
};
</script>
<style>
.user_info {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.user_img {
  width: 200rpx;
  height: 200rpx;
  border-radius: 100rpx;
  margin: 100rpx 0;
}
.user_name{
  font-size: 40rpx;
  font-weight: bold;
  margin: 10rpx 0;
}
</style>