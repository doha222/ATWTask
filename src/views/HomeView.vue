<template>
  <div class="home">
    <div class="app-container">
    <navbar class="trans-nav"></navbar>
    <banner></banner>
  </div>

  <section1></section1>
  <section2></section2>
  <collections></collections>
  <myfooter></myfooter>
  </div>
</template>

<script>
import navbar from "../components/navbar.vue";
import banner from "../components/banner.vue";
import section1 from "../components/section1.vue";
import section2 from "../components/section2.vue";
import collections from "../components/collections.vue";
import myfooter from "../components/myfooter.vue";
export default {
  components: {
    navbar,
    banner,
    section1,
    section2,
    collections,
    myfooter,
    // HomeView
  },
};
</script>
<style>
.app-container {
  position: relative;
}

.trans-nav {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1;
  background-color: (0, 0, 0, 0.8);
}
body {
  margin: 0px;
  /* padding: 0; */
  font-family: "Poppins", sans-serif;
  background-color: #816797;
}


</style>
