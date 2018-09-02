<template>
  <ul id="postList">
    <li class="post-summary" v-for="item in posts" :key="item.id">
      <img :src="image_src" />
      <div class="post-content">
        <h3>{{ item.title }}</h3>
        <h4>{{ item.date }}</h4>
        {{ item.summary }}
      </div>
    </li>
  </ul>

</template>

<script>
import json from "../assets/json/posts.json";
import image from "../assets/logo.png";
export default {
  name: "PostSummary",
  // props: {
  //   msg: String
  // },
  // el: "#postList",
  data() {
    return {
      posts: json,
      image_src: image
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
h3 {
  margin: 0;
  width: 100%;
}

h4 {
  margin: 0 0 8px 0;
  font-size: 14px;
  color: rgba(0, 0, 0, 0.36);
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: flex;
  margin-bottom: 16px;
}

a {
  color: #42b983;
}

img {
  width: 20px;
  height: 20px;
  border-radius: 2px;
}

.post-image {
  width: 96px;
  height: 96px;
  background-color: #ccc;
}

.post-content {
  padding: 0 8px;
  text-align: left;
}
</style>
