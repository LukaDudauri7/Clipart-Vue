<template>
  <div class="center-container">
    <div class="img-container">
      <img src="../assets/region.jpg" class="img-class" />
    </div>
    <div class="timeandfield">
      <div class="field">12.08.2023</div>
      <div class="field">პოლიტიკა</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style scoped>
.center-container {
  margin-top: 40px;
  width: 976px;
  height: 606px;
  background-color: white;
  border-radius: 20px;
}
.img-class {
  width: 952px;
  height: 406px;
  position: relative;
  left: calc((100% - 952px) / 2);
  top: 12px;
  border-radius: 20px;
}
.timeandfield {
    margin-top: 20px;
    display: flex;
    width: 180px;
    justify-content: space-evenly;
    margin-left: 12px;
    gap: 12px;
}
.field{
  color:#1D2D35;
  font-weight: 700;
  font-family: "NotoSans";
  line-height: 16px;
  font-size: 12px;
  padding: 6px 8px;
  background-color: #F5F8FF;
  gap: 10px;
  border-radius: 16px;
  width: 85px;
  height: 16px;
}
</style>
