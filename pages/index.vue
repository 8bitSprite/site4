<template>
  <section class="container">
    <AppBar nav="nav here"/>
    <div class="main">
      <PostList/>
      <Sidebar/>
    </div>
    <Footer/>
  </section>
</template>

<script>
import image from "assets/fonts/Pixellium.ttf";
import AppBar from "@/components/AppBar.vue";
import PostList from "@/components/PostList.vue";
import Footer from "@/components/Footer.vue";
import Sidebar from "@/components/Sidebar.vue";

export default {
  components: {
    AppBar,
    PostList,
    Footer,
    Sidebar
  }
}
</script>

<style lang="stylus">
@font-face {
  font-family: '8bit';
  src: local('8bit'), url('~assets/fonts/Pixellium.ttf');
  format('truetype');
}

#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.main {
  display: flex;
  width: 85%;
  justify-content: space-between;
  max-width: 800px;
  margin: auto;
  padding: 24px 0;
  min-height: calc(100vh);
}
</style>

