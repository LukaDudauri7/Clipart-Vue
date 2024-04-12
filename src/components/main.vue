<template>
  <div>
    <div class="center-container">
      <div class="img-container">
        <img src="../assets/region.jpg" class="img-class" />
      </div>
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
  width: 1200px;
  height: 600px;
  background-color: white;
  border-radius: 20px;
  position: absolute;
  left: calc((100% - 1200px) / 2);
}
.img-class {
  height: 450px;
  width: 1172px;
  position: absolute;
  left: calc((100% - 1172px) / 2);
  top: 12px;
  border-radius: 20px;
}
</style>
