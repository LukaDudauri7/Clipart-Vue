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
            <a class="navbar-item" href="#">ბიზნესი & ეკონომიკა</a>
            <a class="navbar-item" href="#">სხვა</a>
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
      // isMenuOpen: false
    };
  },
  // methods: {
  //   toggleMenu() {
  //     this.isMenuOpen = !this.isMenuOpen;
  //   }
  // }
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
  max-width: 90%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.navbar-logo {
  max-height: 2rem;
}
.navbar-menu {
  display: flex;
  gap: 60px;
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
  gap: 20px;
}
img {
  cursor: pointer;
}
.left-side{
  display: flex;
  gap: 18px;
}
.right-side{
  display: flex;
  gap: 12px;
  align-items: center;
}
</style>
