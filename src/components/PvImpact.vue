<template>
  <section class="impact">
    <img src="../assets/impact2.png" alt="" />
    <h1>VIBRE MAIS ALTO</h1>
  </section>
</template>

<script>
export default {
  name: "PvImpact",
  computed: {
    mobile() {
      return window.innerWidth <= 640;
    },
  },
};
</script>

<style lang="scss" scoped>
.impact {
  display: flex;
  position: relative;
  width: 100%;
  height: 50vh;

  @media screen and (max-width: 640px) {
    height: 70vh;
  }

  img {
    width: 100%;
    object-fit: cover;
  }

  h1 {
    position: absolute;
    top: 50%;
    left: 0;
    right: 0;
    text-align: center;
    font-size: 4.86vw;
    transform: translate(0, -50%);

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      font-size: 5.86vw;
    }

    @media screen and (max-width: 640px) {
      font-size: 9vw;
    }
  }
}
</style>
