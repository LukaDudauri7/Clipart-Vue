<template>
  <HeaderComponent />
  <div class="center-component">
    <MainComponent />
    <NewsComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/header.vue";
import MainComponent from "./components/main.vue";
import NewsComponent from "./components/news.vue";
export default {
  name: "App",
  components: {
    HeaderComponent,
    MainComponent,
    NewsComponent,
  },
};
</script>

<style>
@font-face {
  font-family: "NotoSans";
  src: url("./fonts/NotoSansGeorgian.ttf") format("woff2");
}
html {
  height: 100vh;
  width: 100vw;
  background-color: #f0f4f5;
}
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f0f0f0;
  text-align: center;
  width: 100%; */
}
body {
  margin: 0;
  padding: 0;
  /* min-height: 100vh; */
}
.center-component {
  display: flex;
  justify-content: center;
  gap: 30px;
}
</style>

