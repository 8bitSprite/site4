<template>
  <div id="logo">
    <img :src="image_src">
  </div>
</template>

<script>
import image from "../assets/logo.png";
export default {
  name: "AnimLogo",
  data: function() {
    return {
      image_src: image
    };
  }
};
</script>
<style scoped>
#logo {
  width: 52px;
  height: 52px;
  display: flex;
  align-items: center;
  justify-content: center;
  /* background-color: #999; */
  /* border-radius: 36px;
    border: 2px solid rgba(0, 0, 0, .16) */
}
img {
  height: 32px;
  width: 32px;
}
</style>
