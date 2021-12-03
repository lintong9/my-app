<template>
  <div class="userInfo">
    <img v-if=userInfo.img :src=userInfo.img alt="" />
    <div class="user-nickName">
      {{ userInfo.name }}
    </div>
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