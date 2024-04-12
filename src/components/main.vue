<template>
  <div class="center-container">
    <div class="img-container">
      <img src="../assets/region.jpg" class="img-class" />
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
</style>
