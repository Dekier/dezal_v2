<template>
  <div class="Navbar__header">
    <div class="Navbar__main-container">
      <div class="Navbar__secound-container">
        <nuxt-link to="/rolety" class="Navbar__logo-transition">
          <nuxt-icon name="logo-dark" class="Navbar__svg-logo" filled />
        </nuxt-link>
        <div class="Navbar__links-container">
          <nuxt-link to="/rolety" class="Navbar__links">Oferta</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Szkolenia</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Wiedza</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Case study</nuxt-link>
        </div>
        <nuxt-link to="/rolety" class="Navbar__link-contact"
          >Skontaktuj się</nuxt-link
        >

        <button
          type="button"
          class="Navbar__hamburger-container"
          @click="changeActiveHamburger()"
        >
          <div
            class="Navbar__hamburger-line"
            :class="{
              'Navbar__hamburger-line--active-left': isActiveHamburger,
            }"
          ></div>
          <div
            class="Navbar__hamburger-line"
            :class="{
              'Navbar__hamburger-line--active-none': isActiveHamburger,
            }"
          ></div>
          <div
            class="Navbar__hamburger-line"
            :class="{
              'Navbar__hamburger-line--active-right': isActiveHamburger,
            }"
          ></div>
        </button>
      </div>
    </div>
  </div>
</template>
<script setup>
const isActiveHamburger = ref(false);
const changeActiveHamburger = () => {
  isActiveHamburger.value = !isActiveHamburger.value;
};
</script>
<style lang="scss" scoped>
@import "Navbar";
</style>
