<template>
  <transition>
    <nav v-show="!navbarHidden">
      <img src="../assets/logo.png" alt="logo" height="120" />
      <ul>
        <li>
          <a href=""><ion-icon name="location"></ion-icon></a>
        </li>
        <li>
          <a href=""><ion-icon name="storefront"></ion-icon></a>
        </li>
      </ul>
    </nav>
  </transition>
</template>

<script>
export default {
  name: "PvNavBar",
  data() {
    return {
      navbarHidden: false,
      prevScrollpos: window.pageYOffset,
    };
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  unmounted() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      const currentScrollPos = window.pageYOffset;

      console.log(window.innerWidth);
      if (window.innerWidth > 640) {
        if (window.pageYOffset < 50) {
          document.querySelector("img").height = 120;
          console.log(document.querySelector("img"));
        } else {
          document.querySelector("img").height = 70;
        }
      }

      if (this.prevScrollpos > currentScrollPos) {
        // o usuário está rolando para cima
        this.navbarHidden = false;
      } else {
        // o usuário está rolando para baixo
        this.navbarHidden = true;
      }
      this.prevScrollpos = currentScrollPos;
    },
  },
};
</script>

<style scoped lang="scss">
nav {
  position: fixed;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 6rem;
  background-color: #000;
  border-bottom: 1px #fff solid;

  @media screen and (max-width: 640px) {
    padding: 1rem 2em;
  }

  img {
    cursor: pointer;
    transition: all 0.6s ease;

    @media screen and (max-width: 640px) {
      height: 60px;
    }
  }

  ul {
    display: flex;
    gap: 2rem;
    font-size: 2rem;
    list-style: none;
    text-decoration: none;

    a {
      color: #fff;
    }
  }
}

.v-enter-active,
.v-leave-active {
  transition: opacity 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>
