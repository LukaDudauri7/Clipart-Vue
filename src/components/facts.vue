<template>
  <div class="facts-div">
    <p>ცნობილი ფაქტები</p>
    <div class="facts">
        <FactComponent />
        <FactComponent />
        <FactComponent />
    </div>
  </div>
</template>

<script>
import FactComponent from "./fact.vue";

export default {
  name: "FactsComponent",
  components: {
    FactComponent,
  },
};
</script>

<style scoped>
    .facts-div{
        width: 976px;
        height: 320px;
        border-radius: 16px;
        background-color: white;
        position: relative;
        left: 132px;
        top: 50px;
    }
    p {
        font-family: "NotoSans";
        font-size: 16px;
        line-height: 24px;
        font-weight: 500;
        color: #1D2D35;
        padding: 20px;
    }
    .facts{
        display: flex;
        gap: 8px;
        padding: 12px 12px 16px 12px
    }
</style>
