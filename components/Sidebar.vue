<template>
  <div class="sidebar">
    Stuff
  </div>
</template>

<script>
import PostSummary from "@/components/PostSummary.vue";

export default {
  name: "Sidebar"
  //   props: {
  //     msg: String
  //   },
  //   components: {
  //     PostSummary
  //   }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.sidebar {
  padding: 16px;
  display: flex;
  flex-direction: column;
}

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

.sidebar {
  width: 25%;
  border-left: 1px solid rgba(0, 0, 0, 0.08);
  border-radius: 2px;
  min-height: 56px;
}
</style>
