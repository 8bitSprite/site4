<template>
  <div id="footerWrapper">

    <div id="footer">
      <div id="navLinks">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
      </div>
    </div>


  </div>
</template>

<script>
import AnimLogo from "./AnimLogo";
export default {
  name: "Footer",
  props: {
    nav: String
  },
  components: { AnimLogo }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
#footerWrapper {
  height: 256px;
//   background-color: #ccc;
}

#footer {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 85%;
  max-width: 800px;
  background-color: deepskyblue;
  margin: 0 auto;
  height: 100%;
  border-top: 16px solid rgba(0, 0, 0, .16);
}

.router-link-exact-active {
  color: rgba(0, 0, 0, .86);
  border-bottom: 4px solid rgba(0, 0, 0, .16);
  padding: 16px 12px 12px 12px;
  margin: 0 16px;
  transition: .4s ease-in-out;
  // translate-x: left 20px;
}

a, a:visited {
  color: rgba(0, 0, 0, .56);
  text-decoration: none;
  padding: 16px 12px;  
  margin: 0 16px;
}

a:hover {
  background-color: rgba(0, 0, 0, .04);
}

img {
  height: 42px;
  width: 42px;
}
</style>
