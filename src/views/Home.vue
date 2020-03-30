<template>
  <div class="HomePage-container">
    <Header />
    <Feed />
    <Aside />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Feed from "@/components/Feed";
import Aside from "@/components/Aside";

export default {
  components: {
    Header,
    Feed,
    Aside
  }
};
</script>

<style>
.HomePage-container {
  background-color: #f2f2f2;
  display: grid;
  grid-template-columns: 1fr minmax(auto, 600px) minmax(auto, 278px) 1fr;
  grid-template-rows: 54px 1fr;
  grid-template-areas:
    "header header header header"
    ".  feed side-bar  .";
  grid-column-gap: 30px;
}

/*MEDIA*/

@media (max-width: 870px) {
  .HomePage-container {
    display: grid;
    grid-template-columns: 1fr auto 1fr;
    grid-template-rows: 54px 1fr;
    grid-column-gap: 0;
    grid-template-areas:
      "header header header"
      ".  feed   .";
  }
}

@media (max-width: 400px) {
  .post {
    margin-top: 10px;
  }

  .feed {
    padding-bottom: 10px;
  }
  .main-nav {
    display: none;
  }
}
</style>
