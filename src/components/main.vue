<template>
  <div class="center-container">
    <div class="img-container">
      <div class="swiper">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img src="../assets/MainImages/downtown.jpg" class="img-class" />
          </div>
            <div class="swiper-slide">
          <img src="../assets/MainImages/region.jpg" class="img-class" />
            </div>
            <div class="swiper-slide">
          <img src="../assets/MainImages/buildings.jpg" class="img-class" />
            </div>
            <div class="swiper-slide">
          <img src="../assets/MainImages/chicago.jpg" class="img-class" />
            </div>
        </div>
        <div class="swiper-pagination"></div>
        <div class="swiper-button-prev"></div>
        <div class="swiper-button-next"></div>
        <div class="swiper-scrollbar"></div>
      </div>
    </div>
    <div class="timeandfield">
      <div class="field">12.08.2023</div>
      <div class="field">პოლიტიკა</div>
    </div>
    <div class="main-text">ქვემო ქართლის რეგიონში 20 მლნ ლარამდე ღირებულების ინფრასტრუქტურული პროექტები დაიწყება</div>
    <div class="second-text">განთავსების (ლისტინგის) ორგანიზატორი სომხეთის ბანკი სს “არდშიბანკია”. ობლიგაციის ნომინალი - 1000 USD</div>
  </div>
</template>

<script>
import Swiper from "swiper";
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/pagination";
import "swiper/css/bundle";
import { Navigation, Pagination } from "swiper/modules";
export default {
  name: "MainComponent",
  mounted() {
    new Swiper(".swiper", {
      modules: [Navigation, Pagination],
      pagination: {
        el: ".swiper-pagination",
      },
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
      },
      scrollbar: {
        el: ".swiper-scrollbar",
      },
    });
  },
};
</script>

<style>
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
.field {
  color: #1d2d35;
  font-weight: 700;
  font-family: "NotoSans";
  line-height: 16px;
  font-size: 12px;
  padding: 6px 8px;
  background-color: #f5f8ff;
  gap: 10px;
  border-radius: 16px;
  width: 85px;
  height: 16px;
}
.main-text {
  font-family: "NotoSans";
  font-weight: 600;
  line-height: 40px;
  font-size: 24px;
  padding-left: 12px;
  padding-top: 5px;
}
.second-text {
  font-family: "NotoSans";
  font-weight: 400;
  line-height: 24px;
  font-size: 16px;
  padding-left: 12px;
}
.swiper-button-prev, .swiper-button-next {
  width: 80px;
  height: 80px;
  background-image: url('../assets/ArrowL.png');
  background-size: cover;
}
.swiper-button-next {
  background-image: url('../assets/ArrowR.png');
}
.swiper-button-next:after,.swiper-button-prev:after{
  display: none;
}
.swiper-pagination-bullet {
    background-color: white;
}
.swiper-pagination-bullet-active{
  width: 24px;
  height: 8px;
  border-radius: 64px;
  background-color: white;
}
.swiper-scrollbar{
  display: none;
}

</style>
