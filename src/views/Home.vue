<template>
  <div class="HomePage">
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
.HomePage {
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
  .HomePage {
    background-color: #f2f2f2;
    display: grid;
    grid-template-columns: 1fr auto 1fr;
    grid-template-rows: 54px 1fr;
    grid-column-gap: 0;
    grid-template-areas:
      "header header header"
      ".  feed   .";
  }

  .main-nav {
    display: none;
  }

  .side-bar {
    display: none;
  }

  .search-form {
    display: none;
  }

  .header-container {
    padding: 0 10px;
    max-width: 600px;
    margin: 0 auto;
  }
}

@media (max-width: 400px) {
  .header-container {
    justify-content: center;
  }

  .post {
    margin-top: 10px;
  }

  .feed {
    padding-bottom: 10px;
  }
}
</style>
