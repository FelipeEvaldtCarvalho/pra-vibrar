<template>
  <pv-nav-bar />
  <pv-banner />
  <pv-impact />
  <pv-title-text>
    <template v-slot:title>Descubra novas formas de prazer</template>
    <template v-slot:text
      >Prazer livre e desconstruído só aqui na Pra Vibrar oferecemos uma enorme
      variedade de brinquedinhos, lingeries, cosméticos, itens de cuidados
      íntimos, BDSM & muitoooo mais!</template
    >
  </pv-title-text>
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
import PvTitleText from "./components/PvTitleText.vue";

export default {
  name: "App",
  components: {
    PvNavBar,
    PvBanner,
    PvImpact,
    PvCategory,
    PvLocation,
    PvFooter,
    PvTitleText,
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
body {
  background-color: #000;
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
.bg-white {
  background-color: #fff;
}
.c-gray {
  color: #c6c6c6;
}
.c-white {
  color: #fff;
}
.c-black {
  color: #000;
}
</style>
