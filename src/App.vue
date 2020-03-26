<template>
  <div id="app">
    <Header/>
    <Feed/>
    <Aside/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Feed from "./components/Feed";
import Aside from "./components/Aside";
export default {
  name: "App",
  components: {
    Header,
    Feed,
    Aside
  }
};
</script>

 <style>
@import url("./css/container-style.css");
@import url("https://fonts.googleapis.com/css?family=Bungee+Shade|Oswald:400,500,600|Roboto:500&display=swap&subset=cyrillic");
</style>
