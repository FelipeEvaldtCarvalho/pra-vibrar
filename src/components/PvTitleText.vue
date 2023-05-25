<template>
  <section class="bg-black">
    <h1><slot name="title"></slot></h1>
    <p class="c-gray"><slot name="text"></slot></p>
  </section>
</template>

<script>
export default {
  name: "PvTitleText",
};
</script>

<style lang="scss" scoped>
section {
  padding: 8vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 4.5vw;

  @media screen and (max-width: 1007px) and (min-width: 641px) {
    padding: 9vw;
  }

  @media screen and (max-width: 640px) {
    padding: 13vw 8vw;
  }

  h1 {
    font-size: 4.66vw;
    font-weight: 700;
    text-align: center;
    text-transform: uppercase;
    width: 60vw;
    overflow-wrap: break-word;
    word-wrap: break-word;
    word-break: break-word;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      width: 60vw;
      font-size: 4vw;
    }

    @media screen and (max-width: 640px) {
      font-size: 5.5vw;
      width: initial;
    }
  }

  p {
    font-size: 2.9vw;
    font-weight: 300;
    text-align: center;

    @media screen and (max-width: 1007px) and (min-width: 641px) {
      font-size: 2.6vw;
    }

    @media screen and (max-width: 640px) {
      font-size: 5vw;
    }
  }
}
</style>
