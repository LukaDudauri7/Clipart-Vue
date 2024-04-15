<template>
  <div class="fact-div">
    <img src="../assets/pic.png"/>
    <p>20 მლნ ლარამდე ღირებულების პროექტები იწყება</p>
  </div>
</template>

<script>

export default {
  name: "FactComponent"
};
</script>

<style scoped>
.fact-div{
    width: 312px;
    height: 204px;
    border-radius: 20px;
    background-color: #F5F8FF;
}
img{
    position: relative;
    left: calc((100% - 288px)/2);
    top: 10px;
}
p{
    font-family: "NotoSans";
    font-size: 16px;
    line-height: 24px;
    font-weight: 500;
    color: #1D2D35;
    padding-left: 20px;
    width: 280px;
}
</style>
