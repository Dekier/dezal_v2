<template>
  <div class="Header__main-container">
    <div class="Header__main-title-container">
      <div class="Header__background">
        <nuxt-icon
          name="webmetric-logo"
          filled
          class="Header__svg-background"
        />
      </div>
      <div class="Header__secound-container">
        <div class="Header__title-container">
          <div class="Header__subtitle-container">
            <span>Agencja UX/UI/CRO</span>
          </div>
          <h1 class="Header__title">Rozwijamy produkty cyfrowe łącząc:</h1>
          <ul class="Header__list">
            <li class="Header__row">
              <nuxt-icon name="circle" class="Header__circle" filled />
              <p class="Header__list-item">
                pozyskiwanie danych o użytkownikach (UX)
              </p>
            </li>
            <li class="Header__row">
              <nuxt-icon name="circle" class="Header__circle" filled />
              <p class="Header__list-item">
                pozyskiwanie danych o użytkownikach (UX)
              </p>
            </li>
            <li class="Header__row">
              <nuxt-icon name="circle" class="Header__circle" filled />
              <p class="Header__list-item">
                pozyskiwanie danych o użytkownikach (UX)
              </p>
            </li>
          </ul>
          <div class="Header__reviews-container">
            <div class="Header__reviews-left">
              <span class="Header__span">REVIWED ON</span>
              <nuxt-icon name="logo-dark" class="Header__svg-clutch" filled />
            </div>
            <div class="Header__reviews-right">
              <nuxt-icon name="logo-dark" class="Header__svg-logo" filled />
              <span>5 REVIEWS</span>
            </div>
          </div>
        </div>
        <div class="Header__title-links-container">
          <nuxt-link to="/rolety" class="Header__title-links"
            ><nuxt-icon name="green" class="Header__svg-green" filled /><span
              class="Header__title-span"
              >Projektowanie UI/UX</span
            ></nuxt-link
          >
          <nuxt-link to="/rolety" class="Header__title-links">
            <nuxt-icon name="green" class="Header__svg-green" filled /><span
              class="Header__title-span"
              >Badania UX</span
            >
          </nuxt-link>
          <nuxt-link to="/rolety" class="Header__title-links">
            <nuxt-icon name="green" class="Header__svg-green" filled /><span
              class="Header__title-span"
              >Analityka</span
            ></nuxt-link
          >
        </div>
      </div>
    </div>
    <div class="Header__company-container">
      <span class="Header__company-span">ZAUFALI NAM</span>
      <div class="Header__company-logos">
        <div class="Header__logo-container" v-for="cos in 11" :key="cos">
          <nuxt-icon name="neonail" class="Header__svg-neonail" filled />
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@import "Header";
</style>