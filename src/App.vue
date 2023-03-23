<template>
  <pv-nav-bar />
  <pv-banner />
  <pv-impact />
  <pv-category />
  <pv-location />
  <pv-footer />
</template>

<script>
import PvBanner from "./components/PvBanner.vue";
import PvCategory from "./components/PvCategory.vue";
import PvFooter from "./components/PvFooter.vue";
import PvImpact from "./components/PvImpact.vue";
import PvLocation from "./components/PvLocation.vue";
import PvNavBar from "./components/PvNavBar.vue";

export default {
  name: "App",
  components: {
    PvNavBar,
    PvBanner,
    PvImpact,
    PvCategory,
    PvLocation,
    PvFooter,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  color: #fff;
  font-family: "Montserrat", sans-serif;
}
.c-red {
  color: #ad1b28;
}
.bg-red {
  background-color: #ad1b28;
}
.bg-black {
  background-color: #000;
}
.c-gray {
  color: #c6c6c6;
}
.c-white {
  color: #fff;
}
</style>
