<template>
  <section>
    <div class="video-container">
      <div class="shadow"></div>
      <video autoplay muted loop>
        <source src="../assets/store.mp4" type="video/mp4" />
      </video>
    </div>
    <div class="location">
      <h1>VENHA <span class="c-red">VIBRAR</span> COM A GENTE</h1>
      <h2 class="c-gray">
        Sinta a qualidade dos nossos produtos em primeira mão visitando nossa
        loja.
      </h2>
      <div class="address">
        <ion-icon name="location"></ion-icon>
        <h3>Av. General Flores da Cunha, 4489 Pda 59 - Cachoeirinha - RS</h3>
      </div>
      <a class="btn bg-red" href="">V E N H A</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "PvLocation",
};
</script>

<style lang="scss" scoped>
section {
  background-color: #000;
  .video-container {
    position: relative;
    width: 100%;
    height: 50vw;
    overflow: hidden;

    @media screen and (max-width: 640px) {
      height: 60vh;
    }

    .shadow {
      position: absolute;
      width: 100%;
      height: 50vw;
      -webkit-box-shadow: inset 0px -36px 37px 14px rgba(0, 0, 0, 1);
      -moz-box-shadow: inset 0px -36px 37px 14px rgba(0, 0, 0, 1);
      box-shadow: inset 0px -3vw 3vw 4.2vw rgba(0, 0, 0, 1);

      @media screen and (max-width: 640px) {
        height: 60vh;
      }
    }
    video {
      width: 100%;

      @media screen and (max-width: 640px) {
        height: 100%;
        object-fit: cover;
      }
    }
  }
  .location {
    position: relative;
    top: -15vw;
    display: flex;
    flex-direction: column;
    padding: 0 9vw;

    @media screen and (max-width: 640px) {
      top: -35vw;
    }

    h1 {
      font-size: 5vw;
      text-align: center;
      margin-bottom: 8vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        font-size: 5vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 9vw;
        margin-bottom: 12vw;
      }
    }
    h2 {
      font-size: 2vw;
      letter-spacing: 0.8vw;
      font-weight: 500;
      text-align: center;
      margin-bottom: 5vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        font-size: 2.2vw;
      }

      @media screen and (max-width: 640px) {
        font-size: 4.8vw;
        margin-bottom: 10vw;
      }
    }

    .address {
      display: flex;
      align-items: center;
      gap: 1.5vw;
      width: 40vw;
      margin: 0 auto;
      margin-bottom: 5vw;

      @media screen and (max-width: 640px) {
        flex-direction: column;
        gap: 5vw;
        width: 75vw;
        margin: 0 0;
      }

      ion-icon {
        font-size: 6vw;
        @media screen and (max-width: 640px) {
          font-size: 7vw;
        }
      }
      h3 {
        font-size: 2vw;
        font-weight: 400;
        text-align: center;

        @media screen and (max-width: 640px) {
          font-size: 4vw;
        }
      }
    }

    .btn {
      z-index: 1;
      text-decoration: none;
      padding: 0.83vw 0;
      width: 16.66vw;
      border: none;
      font-size: 0.97vw;
      font-weight: 700;
      text-align: center;
      margin: 0 auto;
      margin-top: 5vw;

      @media screen and (max-width: 1007px) and (min-width: 641px) {
        padding: 1vw 0;
        width: 18.66vw;
        font-size: 1.2vw;
      }

      @media screen and (max-width: 640px) {
        position: relative;
        top: 15vw;
        padding: 2vw 0;
        font-size: 2.5vw;
        width: 40vw;
      }
    }
  }
}
</style>
