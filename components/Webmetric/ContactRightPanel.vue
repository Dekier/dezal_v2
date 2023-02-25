<template>
  <div class="ContactRightPanel__main-container">
    <div class="ContactRightPanel__title-container">
      <span class="ContactRightPanel__title">Napisz do nas</span>
      <strong class="ContactRightPanel__strong">Porozmawiajmy o UX</strong>
    </div>
    <div class="ContactRightPanel__label-container">
      <span class="ContactRightPanel__label">twoje imie</span>
      <input type="text" class="ContactRightPanel__input" />
    </div>
    <div class="ContactRightPanel__label-container">
      <span class="ContactRightPanel__label">E-mail firmowy</span>
      <input type="text" class="ContactRightPanel__input" />
    </div>
    <div class="ContactRightPanel__label-container">
      <span class="ContactRightPanel__label">Twój telefon</span>
      <input type="number" class="ContactRightPanel__input" />
    </div>
    <div class="ContactRightPanel__label-container-big">
      <span class="ContactRightPanel__label">Dodatkowe informacje</span>
      <textarea
        class="ContactRightPanel__input ContactRightPanel__textarea"
        placeholder="Opis projektu, deadline, budżet, NDA"
      />
    </div>
    <div class="ContactRightPanel__footer-container">
      <input type="button" value="Wyślij" class="ContactRightPanel__button" />
      <div class="ContactRightPanel__footer-data">
        <span>Wysyłając wiadomość wyrażasz zgodę na</span>
        <nuxt-link to="/kontakt" class="ContactRightPanel__footer-link"
          >przetwarzanie danych osobowych.</nuxt-link
        >
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@import "ContactRightPanel";
</style>
