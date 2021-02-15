<template>
  <div>
    <Header />
    <Post />
  </div>
</template>

<script>
import Header from "~/components/Header";
import Post from "~/components/Post";
export default {
  components: {
    Header,
    Post
  },
  data() {
    return {
      switch1: true
    };
  }
};
</script>
