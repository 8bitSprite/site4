<template>
  <div class="post-list">
    <!-- <PostSummary msg="Test Post Title"/> -->
    <PostSummary/>
  </div>
</template>

<script>
import PostSummary from "@/components/PostSummary.vue"; 

export default {
  name: "PostList",
  props: {
    msg: String
  },
  components: {
    PostSummary
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.post-list {
  width: 100%;

}
</style>
