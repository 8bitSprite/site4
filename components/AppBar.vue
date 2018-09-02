<template>
  <div id="appBar">
    <div id="mainNav">
      <AnimLogo/>
      <div class="logo-text">8bitSprite</div>
      <!-- use router-link component for navigation. -->
      <!-- specify the link by passing the `to` prop. -->
      <!-- `<router-link>` will be rendered as an `<a>` tag by default -->
      <div id="navLinks">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/about">About</nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
import AnimLogo from "./AnimLogo";
export default {
  name: "AppBar",
  props: {
    nav: String
  },
  components: { AnimLogo }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
#appBar {
  display: flex;
  justify-content: center;
  height: 72px;
  background-color: #fff;
  margin-top: 16px;
  width: 100%;
}

#mainNav {
  font-family: '8bit';
  font-size: 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 85%;
  max-width: 800px;
  height: 100%;
  border-bottom: 1px solid rgba(0, 0, 0, 0.08);
}

#navLinks {
  flex-grow: 2;
  text-align: right;
}

.logo-text {
  border-bottom: 1px solid rgba(0, 0, 0, 0.26);
  color: rgba(0, 0, 0, 0.76);
  height: 32px;
  line-height: 32px;
  border-top: 1px solid rgba(0, 0, 0, 0.26);
}

.router-link {
  padding: 0;
}

.router-link-exact-active {
  color: rgba(0, 0, 0, 0.86);
  border-bottom: 4px solid rgba(0, 0, 0, 0.16);
  padding: 16px 12px 22px 12px;
  margin: 0 16px;
  transition: 0.4s ease-in-out;
}

a, a:visited {
  color: rgba(0, 0, 0, 0.56);
  text-decoration: none;
  padding: 16px 12px;
  margin: 0 16px;
  font-family: Roboto;
  font-size: 1rem;
}

a:hover {
  background-color: rgba(0, 0, 0, 0.04);
}

img {
  height: 42px;
  width: 42px;
}
</style>
