<template>
  <section>
    <div class="banner-text">
      <h1>SINTA ESTÁ VIBRAÇÃO</h1>
      <h2 class="c-gray">
        Aqui na <span class="c-white">Pra Vibrar</span>, provocamos nosso
        público a explorar suas fantasias de uma forma livre e desconstruída.
        Vibração é energia e nós trabalhamos pra te ver
        <span class="c-white">VIBRAR!</span>
      </h2>
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
  padding-bottom: 3.3vw;
  @media screen and (max-width: 1007px) and (min-width: 641px) {
    height: auto;
    min-height: initial;
    padding-top: 150px;
    margin-bottom: -20vw;
    flex-direction: column;
  }
  @media screen and (max-width: 640px) {
    min-height: 100vh;
    flex-direction: column-reverse;
    padding-top: 80px;
    padding-bottom: 20vw;
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
      padding: 0 6.94vw;
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
        font-size: 5vw;
        line-height: 7vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 9vw;
        line-height: 12vw;
        margin-bottom: 5.5vw;
        text-align: center;
      }
    }

    h2 {
      font-size: 2.08vw;
      font-weight: 300;
      line-height: 2.6vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        max-width: 60%;
        font-size: 2.5vw;
        line-height: 3.4vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 6vw;
        line-height: 8vw;
        text-align: center;
      }
    }
  }

  .banner-img {
    display: flex;
    width: 50%;
    padding: 2rem;
    z-index: 0;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      width: 100%;
      position: relative;
      justify-content: flex-end;
      top: -20vw;
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
