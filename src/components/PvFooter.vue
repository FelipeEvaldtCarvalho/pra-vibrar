<template>
  <footer>
    <div class="brand">
      <img src="../assets/logo.png" alt="Logo" />
      <p class="c-gray">
        Nossa loja é discreta e moderna, com atendimento único para uma
        experiência leve e descontraída. Discrição e qualidade são as nossas
        prioridades.
      </p>
    </div>
    <div class="list">
      <span class="list__item--icon">
        <ion-icon class="c-gray" name="call"></ion-icon>
        <p class="c-gray">(51) 989 304 355</p>
      </span>
      <span class="list__item--icon">
        <ion-icon class="c-gray" name="storefront"></ion-icon>
        <p class="c-gray">www.pravibrar.com.br</p>
      </span>
      <span class="list__item--icon">
        <ion-icon class="c-gray" name="mail"></ion-icon>
        <p class="c-gray">pravibrarsexshop@gmail.com</p>
      </span>
      <span class="list__item c-gray">© Pra Vibrar - Sex Shop</span>
      <span class="list__item c-gray">2023 Todos os direitos reservados.</span>
      <span class="list__item c-gray">CNPJ: 25.121.144/0001-27</span>
    </div>
    <span class="social">
      <a href=""><ion-icon name="logo-instagram"></ion-icon></a>
      <a href=""><ion-icon name="logo-whatsapp"></ion-icon></a>
    </span>
  </footer>
</template>

<script>
export default {
  name: "PvFooter",
};
</script>

<style lang="scss" scoped>
footer {
  background-color: #000;
  display: flex;
  padding: 0 6vw 6vw 6vw;
  justify-content: space-between;
  align-items: center;
  position: relative;

  @media screen and (max-width: 640px) {
    flex-direction: column;
    gap: 15vw;
    padding: 0 8vw 25vw 8vw;
  }

  .brand {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2.5vw;
    font-size: 1.1vw;
    width: 34.2vw;
    letter-spacing: 0.3vw;
    text-align: center;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      font-size: 1.3vw;
      width: 40vw;
    }

    @media screen and (max-width: 640px) {
      width: 100%;
      font-size: 3.6vw;
      letter-spacing: 0.9vw;
      gap: 9vw;
    }

    img {
      height: 8vw;

      @media screen and (max-width: 640px) {
        height: 25vw;
      }
    }
  }

  .list {
    display: flex;
    flex-direction: column;
    font-size: 1.1vw;
    text-align: center;
    min-width: 29vw;
    align-items: center;
    letter-spacing: 0.3vw;
    gap: 0.4vw;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      font-size: 1.3vw;
      width: 40vw;
    }

    @media screen and (max-width: 640px) {
      width: 100%;
      font-size: 3.6vw;
      letter-spacing: 0.9vw;
      gap: 1vw;
    }

    &__item--icon {
      display: flex;
      align-items: center;
      gap: 0.8vw;
      margin-bottom: 0.6vw;

      @media screen and (max-width: 640px) {
        flex-direction: column;
        gap: 3vw;
        margin-bottom: 10vw;
      }

      ion-icon {
        font-size: 1.5vw;

        @media screen and (max-width: 640px) {
          font-size: 5vw;
        }
      }
    }
  }

  .social {
    display: flex;
    font-size: 3vw;
    gap: 2vw;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      position: absolute;
      left: 50%;
      transform: translate(-50%);
      top: -8vw;
    }

    @media screen and (max-width: 640px) {
      order: -1;
      font-size: 10vw;
      gap: 15vw;
    }

    a {
      transition: 0.6s all ease;

      &:hover {
        transform: scale(1.15);
      }
    }
  }
}
</style>
