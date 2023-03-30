<template>
  <div
    class="NavBar__main-container"
    :class="{ 'NavBar__main-container--active': isActiveNavbar }"
  >
    <div class="NavBar__center-container">
      <div class="NavBar__left-panel">
        <nuxt-icon name="logo" filled class="NavBar__logo" />
      </div>
      <div class="NavBar__links-container">
        <nuxt-link
          to="/oferta"
          class="NavBar__link"
          :class="{ 'NavBar__link--active': route.name === 'oferta' }"
          >oferta
          <span class="NavBar__icon-container">
            <nuxt-icon
              name="Arrow"
              filled
              class="NavBar__arrow"
              :class="{ 'NavBar__arrow--active': isActiveButton }"
              @click="changeActiveButton()"
            />
          </span>
        </nuxt-link>
        <nuxt-link
          to="/onas"
          class="NavBar__link"
          :class="{ 'NavBar__link--active': route.name === 'onas' }"
          >o nas</nuxt-link
        >
        <nuxt-link
          to="/realizacje"
          class="NavBar__link"
          :class="{ 'NavBar__link--active': route.name === 'realizacje' }"
          >realizacje</nuxt-link
        >
        <nuxt-link
          :class="{ 'NavBar__link--active': route.name === 'produkty' }"
          to="/produkty"
          class="NavBar__link"
          >produkty</nuxt-link
        >
        <nuxt-link
          to="/kontakt"
          class="NavBar__link-yellow"
          :class="{ 'NavBar__link-yellow--active': route.name === 'kontakt' }"
          >kontakt</nuxt-link
        >
      </div>
      <div class="NavBar__right-panel">
        <div class="NavBar__label">
          <div class="NavBar__absolute">
            <nuxt-icon name="loupe" class="NavBar__svg" filled />
          </div>
          <input type="text" placeholder="np. plisy" class="NavBar__input" />
        </div>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
const route = useRoute();
const isActiveNavbar = ref<boolean>(false);
const isActiveButton = ref<boolean>(false);
const changeActiveButton = () => {
  isActiveButton.value = !isActiveButton.value;
};
onMounted(() => {
  document.addEventListener("scroll", () => {
    window.scrollY <= 60
      ? (isActiveNavbar.value = false)
      : (isActiveNavbar.value = true);
  });
});
onBeforeUnmount(() => {
  document.removeEventListener("scroll", () => {
    window.scrollY <= 60
      ? (isActiveNavbar.value = false)
      : (isActiveNavbar.value = true);
  });
});
</script>
<style lang="scss" scoped>
@import "NavBar";
</style>
