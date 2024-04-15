<template>
  <div class="header-container">
    <div class="center_container">
      <div class="navbar-menu">
        <div class="left-side">
          <img src="../assets/Logo.png" />
          <div class="navbar-end">
            <a class="navbar-item" href="#">პოლიტიკა</a>
            <a class="navbar-item" href="#">საზოგადოება</a>
            <a class="navbar-item" href="#">სამართალი</a>
            <a class="navbar-item titlenone" href="#">ბიზნესი & ეკონომიკა</a>
            <div class="dropdown">
              <a class="navbar-item" href="#" @click="toggleDropdown">სხვა<span class="arrow-icon"></span></a>
              <div v-if="isDropdownOpen" class="dropdown-content">
                <a href="#">ტექნოლოგიები</a>
                <a href="#">სტარტაპები</a>
                <a href="#">სპორტი</a>
                <a href="#" class="dropdownnone">ბიზნესი & ეკონომიკა</a>
              </div>
            </div>
          </div>
        </div>
        <div class="right-side">
          <img src="../assets/instagram.png" class="navbar-logo" />
          <img src="../assets/facebook.png" class="navbar-logo" />
          <input placeholder="ძიება" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      isDropdownOpen: false,
    };
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
  },
};
</script>

<style scoped>
.header-container {
  background-color: white;
  width: 100%;
  height: 112px;
  display: flex;
  justify-content: center;
}
.center_container {
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar-logo {
  max-height: 2rem;
}
.navbar-menu {
  display: flex;
  gap: 200px;
}
a {
  text-decoration: none;
  color: #657178;
  line-height: 24px;
  font-size: 16px;
  font-weight: 500;
  font-family: "NotoSans";
}
input {
  font-family: "NotoSans";
  font-size: 14px;
  font-weight: 400;
  line-height: 20px;
}
.navbar-end {
  width: 85%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 30px;
  margin-left: 10px;
}
img {
  cursor: pointer;
}
.left-side {
  display: flex;
  gap: 18px;
}
.right-side {
  display: flex;
  gap: 12px;
  align-items: center;
}
input{
  border-radius: 64px;
  padding: 9px;
  background-color: #F5F8FF;
  border: none;
  background-image: url(../assets/search.png);
  background-repeat: no-repeat;
  background-size: 17.4px;
  background-position: 150px;
  cursor: pointer;
}
.dropdown {
  position: relative;
}
.dropdown .dropdown-content {
  display: none;
  flex-direction: column;
  position: absolute;
  z-index: 1;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  padding: 12px 16px;
}
.dropdown:hover .dropdown-content {
  display: flex;
  z-index: 2;
}
.arrow-icon {
  position: absolute;
  background-image: url(../assets/arrow.png);
  background-repeat: no-repeat;
  width: 10px;
  height: 7px;
  top: 8px;
  left: 42px;
}
.dropdownnone{
  display: none;
}
.titlenone{
  display: block;
}
@media screen and (min-width: 768px) and (max-width: 1366px) {
  .dropdownnone{
    display: block;
  }
  .titlenone{
    display: none;
  }
}
</style>
