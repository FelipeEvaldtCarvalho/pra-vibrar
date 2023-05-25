<template>
  <section>
    <div
      v-for="(item, index) in categories"
      :key="index"
      :class="`container-${item.class}`"
    >
      <div :class="`text-${item.class}`">
        <h1>{{ item.title }}</h1>
        <h2 class="c-gray">{{ item.text }}</h2>
        <a :class="item.btnClass" href="">{{ item.btn }}</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "PvCategory",
  data() {
    return {
      categories: [
        {
          title: "VIBRADORES",
          text: "Descubra novas texturas, tamanhos, formatos e sensações.",
          btn: "D E S C U B R A",
          img: "vibra.png",
          class: "vib",
          btnClass: "btn bg-red",
        },
        {
          title: "BDSM",
          text: "Liberte sua imaginação, seja quem quiser, escolha dominar ou se submeter.",
          btn: "L I B E R T E - S E",
          img: "bdsm.png",
          class: "bdsm",
          btnClass: "btn bg-black",
        },
        {
          title: "ACESSÓRIOS",
          text: "Não há limites para a imaginação, experiemente, saia da rotina.",
          btn: "S A I A  D A  R O T I N A",
          img: "acessorio.png",
          class: "acessory",
          btnClass: "btn bg-red",
        },
        {
          title: "COSMÉTICOS",
          text: "Eleve sua experiência com a nossa linha de cosméticos  de alta qualidade.",
          btn: "E X P E R I M E N T E",
          img: "cosmetics.png",
          class: "cosmetics",
          btnClass: "btn bg-black",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
section {
  background-color: #000;
  .btn {
    z-index: 1;
    text-decoration: none;
    padding: 0.83vw 0;
    width: 16.66vw;
    border: none;
    font-size: 0.97vw;
    font-weight: 700;
    text-align: center;
    margin-top: 5vw;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      padding: 1vw 0;
      width: 18.66vw;
      font-size: 1.2vw;
    }

    @media screen and (max-width: 640px) {
      padding: 2vw 0;
      font-size: 2.5vw;
      width: 40vw;
    }
  }
  .container-vib {
    display: flex;
    flex-direction: row-reverse;
    height: 52.77vw;

    @media screen and (max-width: 640px) {
      height: 70vw;
    }

    .text-vib {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding-right: 10vw;
      align-items: flex-end;
      text-align: end;
      gap: 3vw;

      @media screen and (max-width: 640px) {
        width: 70%;
        position: relative;
      }

      h1 {
        font-size: 5.66vw;
        font-weight: 700;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 5.86vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 9vw;
        }
      }

      h2 {
        font-size: 2.9vw;
        font-weight: 300;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 2.6vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 4.4vw;
        }
      }
    }

    .img-vib {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;

      @media screen and (max-width: 640px) {
        width: 30%;
        position: relative;
      }

      img {
        width: 100%;
        padding: 0 3vw;

        @media screen and (max-width: 640px) {
          width: 50vw;
          position: absolute;
          left: 0;
          padding: 0;
        }
      }
    }
  }
  .container-bdsm {
    display: flex;
    height: 52.77vw;
    background-color: #ad1b28;
    overflow: hidden;

    @media screen and (max-width: 640px) {
      height: 70vw;
    }

    .text-bdsm {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding-left: 10vw;
      gap: 3vw;

      @media screen and (max-width: 640px) {
        width: 70%;
        position: relative;
      }

      h1 {
        font-size: 5.66vw;
        font-weight: 700;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 5.86vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 9vw;
        }
      }

      h2 {
        font-size: 2.9vw;
        font-weight: 300;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 2.6vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 4.4vw;
        }
      }
    }

    .img-bdsm {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;

      @media screen and (max-width: 640px) {
        width: 30%;
        position: relative;
      }

      img {
        width: 100%;
        margin-bottom: 4vw;

        @media screen and (max-width: 640px) {
          width: 70vw;
          transform: scaleX(-1);
          position: absolute;
          right: -24vw;
        }
      }
    }
  }
  .container-acessory {
    display: flex;
    flex-direction: row-reverse;
    height: 52.77vw;

    @media screen and (max-width: 640px) {
      height: 70vw;
    }

    .text-acessory {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding-right: 10vw;
      align-items: flex-end;
      text-align: end;
      gap: 3vw;

      @media screen and (max-width: 640px) {
        width: 70%;
        position: relative;
      }

      h1 {
        font-size: 5.66vw;
        font-weight: 700;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 5.86vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 9vw;
        }
      }

      h2 {
        font-size: 2.9vw;
        font-weight: 300;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 2.6vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 4.4vw;
        }
      }
    }

    .img-acessory {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;

      @media screen and (max-width: 640px) {
        width: 30%;
        position: relative;
      }

      img {
        width: 100%;
        margin-bottom: 4vw;

        @media screen and (max-width: 640px) {
          width: 55vw;
          position: absolute;
          left: -5vw;
          bottom: 5vw;
          transform: rotate(20deg);
        }
      }
    }
  }
  .container-cosmetics {
    display: flex;
    height: 52.77vw;
    background-color: #ad1b28;
    overflow: hidden;

    @media screen and (max-width: 640px) {
      height: 70vw;
    }

    .text-cosmetics {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding-left: 10vw;
      gap: 3vw;

      @media screen and (max-width: 640px) {
        width: 70%;
        position: relative;
      }

      h1 {
        font-size: 5.66vw;
        font-weight: 700;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 5.86vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 9vw;
        }
      }

      h2 {
        font-size: 2.9vw;
        font-weight: 300;

        @media screen and (max-width: 1007px) and (min-width: 641px) {
          font-size: 2.6vw;
        }

        @media screen and (max-width: 640px) {
          font-size: 4.4vw;
        }
      }
    }

    .img-cosmetics {
      width: 50%;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;

      @media screen and (max-width: 640px) {
        width: 30%;
        position: relative;
      }

      img {
        height: 100%;
        object-fit: contain;

        @media screen and (max-width: 640px) {
          position: absolute;
          transform: scaleX(-1);
        }
      }
    }
  }
}
</style>
