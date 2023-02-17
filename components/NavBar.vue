<template>
  <div class="NavBar__main-container">
    <nuxt-link to="/" class="NavBar__Logo">
      <div class="NavBar__logo">
        <img src="../img/logo.jpg" class="NavBar__Logo" alt="logo kfc" /></div
    ></nuxt-link>
    <div class="NavBar__links-container">
      <nuxt-link to="/rolety" class="NavBar__link">ROLETY</nuxt-link>
      <nuxt-link to="/zaluzje" class="NavBar__link">ŻALUZJE</nuxt-link>
      <nuxt-link to="/kontakt" class="NavBar__link">KONTAKT</nuxt-link>
      <nuxt-link to="/galeria" class="NavBar__link">GALERIA</nuxt-link>
      <nuxt-link to="/webmetric" class="NavBar__link">webmetric</nuxt-link>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "NavBar";
</style>
