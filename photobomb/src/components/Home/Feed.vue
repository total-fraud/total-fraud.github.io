<template>
  <section class="feed">
    <Post v-for="post in posts" :key="post.id" v-bind:post="post" />
  </section>
</template>

<script>
import Post from "@/components/Post";

export default {
  components: {
    Post
  },
  data() {
    return {
      posts: [
        {
          id: 1,
          name: "PusPus",
          content: require("@/assets/cat_jazz.jpg"),
          likes: "45,000",
          comments: [
            {
              id: 1,
              name: "Sebek ",
              text: " wow such a cool cat"
            },
            {
              id: 2,
              name: " AntiSebek ",
              text: " WTF MAN, THAT`S MAH BLINY"
            },
            {
              id: 3,
              name: "TrueSebek ",
              text: " 😻😻😻😻😻😻😻😻😻😻😻😻😻😻😻"
            }
          ]
        },
        {
          id: 2,
          name: "Ginzburg",
          content: "https://picsum.photos/500/500",
          likes: "58,000",
          comments: [
            {
              id: 1,
              name: "Sebek ",
              text: " wow such a cool... whatever"
            },
            {
              id: 2,
              name: " AntiSebek ",
              text: " WTF MAN, THAT`S MAH"
            },
            {
              id: 3,
              name: "TrueSebek ",
              text: "  😡 "
            }
          ]
        },
        {
          id: 3,
          name: "Carlos",
          content: "https://www.placecage.com/gif/500/500",
          likes: "4,000",
          comments: [
            {
              id: 1,
              name: "Sebek ",
              text: " stay at home nick"
            },
            {
              id: 2,
              name: " AntiSebek ",
              text: " WOW THAT`S MAH GIF!!! GIVE IT BACK MAN"
            },
            {
              id: 3,
              name: "TrueSebek ",
              text: " 😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎😎"
            }
          ]
        }
      ]
    };
  }
};
</script>

<style scoped>
.feed {
  background-color: #fafafa;
  padding-bottom: 60px;
  max-width: 600px;
  grid-area: feed;
  justify-self: end;
}
</style>
