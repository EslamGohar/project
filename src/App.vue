<template>
  <navbar />
  <navgation />
  <breadcrumb />
  <side-bar />
  <search-product />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Navgation from "./components/Navgation.vue";
import SideBar from "./components/SideBar.vue";
import Breadcrumb from "./components/Breadcrumb.vue";
import SearchProduct from "./components/SearchProduct.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Navgation,
    Breadcrumb,
    SideBar,
    SearchProduct,
  },
};
</script>

<style>
* {
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  min-height: 100vh;
  font-family: "Montserrat", sans-serif;
  background-color: #f9f9f9;
  color: #4f759b;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
