<template>
  <div id="app">
    <Navbar />
    <router-view />
  </div>
</template>

<script>
import Navbar from "@/layouts/Navbar";
export default {
  components: {
    Navbar
  },
};
</script>

<style Navbarlang="scss">
@import "./fonts/_fonts.scss";

@import "./styles/main.scss";
</style>
