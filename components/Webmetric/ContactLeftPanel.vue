<template>
  <div class="ContactLeftPanel__left-panel">
    <div class="ContactLeftPanel__title">
      <span>
        Szukasz zespołu do stworzenia lub rozwoju produktu cyfrowego, chcesz go
        zbadać i wdrożyć według najlepszych standardów?</span
      >
      <strong class="ContactLeftPanel__strong">
        To dobrze, że tu jesteś.</strong
      >
    </div>
    <div class="ContactLeftPanel__person-data-container">
      <div class="ContactLeftPanel__img-container">
        <img
          src="../../public/assets/img/person.jpg"
          alt="person"
          class="ContactLeftPanel__img"
        />
      </div>
      <div class="ContactLeftPanel__person-data">
        <h1 class="ContactLeftPanel__person-title">Filip Adamus</h1>
        <nuxt-link to="/kontakt" class="ContactLeftPanel__link"
          ><span>f.adamus@webmetric.com</span>
          <div class="ContactLeftPanel__link-underline" />
        </nuxt-link>
        <nuxt-link
          to="/kontakt"
          class="ContactLeftPanel__link ContactLeftPanel__person-margin"
          ><span>+48 537 401 467</span>
          <div class="ContactLeftPanel__link-underline"
        /></nuxt-link>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@import "ContactLeftPanel";
</style>
