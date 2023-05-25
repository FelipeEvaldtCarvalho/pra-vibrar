<template>
  <section class="impact">
    <a class="btn bg-white c-black" href="">LOJA VIRTUAL</a>
  </section>
</template>

<script>
export default {
  name: "PvImpact",
};
</script>

<style lang="scss" scoped>
.impact {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding-bottom: 10vh;
  align-items: center;
  width: 100%;
  height: 75vh;
  background-image: url("../assets/impact2.png");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  filter: saturate(0);

  @media screen and (max-width: 640px) {
    height: 50vh;
  }

  a {
    letter-spacing: 0.2vw;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      letter-spacing: 0.4vw;
    }

    @media screen and (max-width: 640px) {
      font-size: 9vw;
    }
  }
  .btn {
    height: 40px;
    text-decoration: none;
    padding: 12px 0;
    width: 260px;
    border: none;
    -webkit-box-shadow: 0px 0px 0px 1px rgba(0, 0, 0, 1);
    -moz-box-shadow: 0px 0px 0px 1px rgba(0, 0, 0, 1);
    box-shadow: 0px 0px 0px 1px rgba(0, 0, 0, 1);
    letter-spacing: 20%;
    font-size: 14px;
    font-weight: 700;
    text-align: center;
  }
}
</style>
