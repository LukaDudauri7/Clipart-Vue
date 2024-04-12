<template>
  <div class="news-container">
    <h1>ყველა სიახლე</h1>
    <div class="paragraphs">
      <div v-for="index in 30" :key="index">
        <ParagraphComponent />
      </div>
    </div>
  </div>
</template>

<script>
import ParagraphComponent from "./paragraph.vue";
export default {
  name: "NewsComponent",
  components: {
    ParagraphComponent,
  },
};
</script>

<style scoped>
.news-container {
  margin-top: 40px;
  width: 304px;
  height: 606px;
  background-color: white;
  border-radius: 20px;
  overflow: hidden;
}
.paragraphs {
  overflow: auto;
  height: calc(100% - 60px); /* Adjusted height to accommodate h1 */
}
h1 {
  font-size: 20px;
  line-height: 28px;
  font-family: "NotoSans";
  color: #1d2d35;
  margin-left: 20px;
  margin-top: 20px;
}
::-webkit-scrollbar {
  width: 4px;
}
::-webkit-scrollbar-thumb {
  background: #657178;
  border-radius: 6px;
}
</style>
