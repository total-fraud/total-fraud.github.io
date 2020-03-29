<template>
  <section class="feed">
    <Post />
  </section>
</template>

<script>
import Post from "@/components/Post";

export default {
  components: {
    Post
  }
};
</script>

<style scoped>
.feed {
  padding-bottom: 60px;
  max-width: 600px;
  grid-area: feed;
  justify-self: end;
}
</style>
