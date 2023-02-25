<template>
  <div class="Payments__buy-container">
    <div class="Payments__company-container">
      <p class="Payments__company-name">od doragdsklep</p>
      <div class="Payments__row">
        <span class="Payments__small-text">Firma</span>
        <span class="Payments__wall">|</span>
        <a
          href="#aboutSaller"
          class="Payments__small-text Payments__small-text--green Payments__noDecoration"
          >Poleca</a
        >
      </div>
    </div>
    <div class="Payments__payment-container">
      <h1 class="Payments__title">
        TEVOUP ACMER R10 Obudowa do grawerki laserowej
      </h1>
      <div class="Payments__row">
        <span class="Payments__number--big">359,</span>
        <span class="Payments__number">00 zł</span>
      </div>
      <hr class="Payments__line" />
      <p class="Payments__paragraf">Liczba sztuk</p>
      <div class="Payments__row">
        <button class="Payments__button" @click="minus">-</button>
        <input v-model="count" class="Payments__input" />
        <button class="Payments__button" @click="plus">+</button>
        <p class="Payments__small-text Payments__middle">z 33 sztuk</p>
      </div>
      <button class="Payments__button-orange">DODAJ DO KOSZYKA</button>
      <button class="Payments__button-orange">KUP TERAZ</button>
    </div>
  </div>
</template>
<script setup>
const minus = () => {
  count.value--;
};
const plus = () => {
  count.value++;
};
const count = ref(0);
</script>
<style lang="scss" scoped>
@import "Payments";
</style>
