<template>
  <div class="news">
    <div class="news-header">
      <img src="../assets/Vector.png" />
      <div class="time">7:30</div>
      <div class="rectangle"></div>
      <div class="time">02.01.2023</div>
    </div>
    <p>დღეიდან ასაწონად განკუთვნილ პოლიეთილენის პარკები აიკრძალა</p>
    <div class="line"></div>
  </div>
</template>

<script>
export default {
  name: "ParagraphComponent",
};
</script>

<style scoped>
.news{
  margin-top: 25px;
}
.news-header {
  display: flex;
  width: 272px;
  margin-left: 20px;
  gap: 5px;
  align-items: center
}
p {
  font-weight: 400;
  color: #1d2d35;
  font-size: 14px;
  font-family: "NotoSans";
  line-height: 20px;
  width: 272px;
  text-align: left;
  margin-left: 20px;
  margin-top: 0px;
}
.time{
  color: #585EE3;
  font-weight: 700;
  font-size: 12px;
  line-height: 16px;
  font-family: "NotoSans";
}
.rectangle{
  background-color: #585EE3;
  width: 4px;
  height: 4px;
  border-radius: 50%;
}
</style>
