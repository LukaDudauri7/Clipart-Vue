<template>
  <HeaderComponent />
  <MainComponent />
</template>

<script>
import HeaderComponent from './components/header.vue'
import MainComponent from './components/main.vue'
export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent
  }
}
</script>

<style>
@font-face {
  font-family: 'NotoSans';
  src: url('./fonts/NotoSansGeorgian.ttf') format('woff2')
}
html{
  height: 100vh;
  width: 100vw; 
  background-color: #F0F4F5;
}
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #f0f0f0;
  text-align: center;
  width: 100%; */
}
body{
  margin: 0;
  padding: 0;
  /* min-height: 100vh; */
}
</style>

