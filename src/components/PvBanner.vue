<template>
  <section>
    <div class="banner-text">
      <h1>AQUI O PRAZER <span class="c-red">VIBRA</span> EM CADA DETALHE</h1>
      <h2 class="c-gray">Desconstrua padrões</h2>
      <h2 class="c-gray">Liberte seus <span class="c-white">fetiches</span></h2>
      <h2 class="c-gray">Explore o <span class="c-white">prazer</span></h2>
      <h2 class="c-gray">Saia da rotina</h2>
      <a class="btn bg-red" href="">D E S C U B R A</a>
    </div>
    <div class="banner-img">
      <img src="../assets/bannerBg.png" alt="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "PvBanner",
};
</script>

<style lang="scss" scoped>
section {
  height: auto;
  min-height: 100vh;
  background-color: #000;
  display: flex;
  align-items: center;
  padding-top: 110px;
  padding-bottom: 3rem;
  @media screen and (max-width: 1007px) and (min-width: 641px) {
    min-height: initial;
    flex-direction: column;
  }
  @media screen and (max-width: 640px) {
    min-height: 100vh;
    flex-direction: column-reverse;
    padding-top: 80px;
  }

  .banner-text {
    z-index: 1;
    display: flex;
    width: 50%;
    flex-direction: column;
    padding-left: 6.94vw;
    position: relative;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      width: 100%;
      padding-top: 1rem;
    }

    @media screen and (max-width: 640px) {
      width: 100%;
      padding: 0 8vw;
    }

    h1 {
      font-size: 4.86vw;
      font-weight: 700;
      line-height: 5.6vw;
      margin-bottom: 2.5vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        font-size: 5.86vw;
        line-height: 7vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 9vw;
        line-height: 12vw;
        margin-bottom: 5.5vw;
      }
    }

    h2 {
      font-size: 2.08vw;
      font-weight: 300;
      line-height: 2.6vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        font-size: 2.5vw;
        line-height: 3.4vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 6vw;
        line-height: 8vw;
      }
    }

    .btn {
      margin-top: 5.2vw;
      text-decoration: none;
      padding: 0.83vw 0;
      width: 16.66vw;
      border: none;
      letter-spacing: 20%;
      font-size: 0.97vw;
      font-weight: 700;
      text-align: center;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        padding: 1vw 0;
        width: 18.66vw;
        font-size: 1.2vw;
      }

      @media screen and (max-width: 640px) {
        padding: 2vw 0;
        width: 100%;
        font-size: 3.5vw;
        margin-top: 12vw;
      }
    }
  }

  .banner-img {
    display: flex;
    width: 50%;
    padding: 2rem;
    z-index: 0;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      position: absolute;
      right: 6%;
      top: 19%;
    }

    @media screen and (max-width: 640px) {
      width: 100%;
      padding: 0;
    }

    img {
      width: 100%;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        width: 50vw;
      }
    }
  }
}
</style>
