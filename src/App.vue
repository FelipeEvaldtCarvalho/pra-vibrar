<template>
  <pv-nav-bar />
  <pv-banner />
  <div class="teste-app">
    <h1>adsdasd asd asd as</h1>
    <h1>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi tenetur
      odit, maiores odio qui magni corrupti sint repudiandae, perferendis
      aperiam dolores fuga laboriosam beatae a modi itaque accusamus iste
      nesciunt.
    </h1>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae asperiores
      unde eos impedit. Minus, quia numquam deserunt placeat impedit
      perspiciatis. Ipsum iusto ipsa fugiat, debitis itaque aliquam id quam ad
      minus ut soluta architecto eius harum dolore dolor quod placeat doloribus
      sit commodi, necessitatibus illum! Et quibusdam ea consequuntur ratione
      vero amet? Ex vero adipisci quibusdam atque necessitatibus aspernatur
      recusandae qui maiores explicabo veniam aut aperiam esse beatae maxime
      molestiae consectetur tenetur iure, tempora quod sint. Laboriosam
      doloribus quidem, obcaecati deleniti qui, beatae ea ex omnis maiores
      officiis libero recusandae quaerat nisi enim. Sit eum debitis repellat at
      eius expedita. Provident, saepe dolorem nam temporibus tempora officia
      corporis dignissimos distinctio rerum suscipit blanditiis hic, animi
      possimus sapiente quidem consectetur! Earum, in nisi asperiores aperiam
      voluptate minima, deserunt, dolorum suscipit recusandae quaerat rem soluta
      libero eligendi veritatis omnis fugit ex magni est nam sed ipsum! Odio
      officiis tempora culpa similique, aliquid fugiat ipsa. Tempore, explicabo
      doloribus delectus in quos odio error molestias? Ut, dolorem minima!
      Voluptatem autem omnis labore, laudantium iusto ex qui quos nobis illum ut
      aliquam, aliquid ea quam? Eligendi voluptate odit, beatae perspiciatis
      natus aliquam voluptatum illum eos iusto facilis? Laborum iusto sint
      explicabo dignissimos placeat voluptatem debitis.
    </p>
  </div>
</template>

<script>
import PvBanner from "./components/PvBanner.vue";
import PvNavBar from "./components/PvNavBar.vue";

export default {
  name: "App",
  components: {
    PvNavBar,
    PvBanner,
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
  color: #9c9c9c;
}
.c-white {
  color: #fff;
}
.teste-app {
  min-height: 150vh;
  padding: 300px 50px;
  background-color: blueviolet;
}
</style>
