<template>
  <div class="Navbar__header">
    <div class="Navbar__main-container">
      <div class="Navbar__secound-container">
        <nuxt-link to="/rolety" class="logo-transition">
          <nuxt-icon name="logo-dark" class="Navbar__svg-logo" filled />
        </nuxt-link>
        <div class="Navbar__links-container">
          <nuxt-link to="/rolety" class="Navbar__links">Oferta</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Szkolenia</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Wiedza</nuxt-link>
          <nuxt-link to="/rolety" class="Navbar__links">Case study</nuxt-link>
        </div>
        <nuxt-link to="/rolety" class="Navbar__link-border"
          >Skontaktuj się</nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import "Navbar";
</style>