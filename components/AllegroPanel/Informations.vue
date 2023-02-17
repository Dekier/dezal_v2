<template>
  <div class="Informations__information-container">
    <div class="Informations__country Informations__bottom-border">
      <div class="Informations__icon"></div>
      <div class="Informations__column">
        <p class="Informations__small-text--dark-Gray">Kraj wysyłki</p>
        <span class="Informations__small-text">Niemcy</span>
      </div>
    </div>
    <a href="faraway" class="Informations__noDecoration">
      <div class="Informations__delivery Informations__bottom-border">
        <div class="Informations__icon"></div>
        <div class="Informations__paragraph-width">
          <p class="Informations__small-text--dark-Gray">Dostawa od 24,99zł</p>
          <span class="Informations__small-text">
            Przewidywana dostawa: śr. 15 lut. -pt. 17 lut. u Ciebie</span
          >
        </div>
        <div class="Informations__svg">
          <nuxt-icon name="arrow" filled />
        </div>
      </div>
    </a>
    <a href="faraway" class="Informations__noDecoration">
      <div class="Informations__refund Informations__bottom-border">
        <div class="Informations__icon"></div>
        <div class="Informations__paragraphs">
          <p class="Informations__small-text--dark-Gray">Zwrot Ograniczony</p>
          <span class="Informations__small-text"
            >14dni na odstąpienie od umowy</span
          >
        </div>
        <div class="Informations__svg">
          <nuxt-icon name="arrow" filled />
        </div>
      </div>
    </a>
    <a href="faraway" class="Informations__noDecoration">
      <div
        class="Informations__guarantee-container Informations__bottom-border"
      >
        <div class="Informations__icon"></div>
        <div class="Informations__guarantee-paragrahps">
          <p class="Informations__small-text--dark-Gray">Gwarancja</p>
          <span class="Informations__small-text">24 miesiące</span>
        </div>
        <div class="Informations__svg">
          <nuxt-icon name="arrow" filled />
        </div>
      </div>
    </a>
    <a href="faraway" class="Informations__noDecoration">
      <div
        class="Informations__complaint-container Informations__bottom-border"
      >
        <div class="Informations__icon"></div>
        <p class="Informations__small-text--dark-Gray">Reklamacja</p>
        <div class="Informations__svg">
          <nuxt-icon name="arrow" filled />
        </div>
      </div>
    </a>
    <a href="faraway" class="Informations__noDecoration">
      <div class="Informations__protect">
        <div class="Informations__icon"></div>
        <div class="Informations__paragraphs">
          <p class="Informations__small-text--dark-Gray">
            Kupujesz z Allegro Protect
          </p>
          <span class="Informations__small-text"
            >100% zakupów ze zwrotem pieniędzy</span
          >
        </div>
        <div class="Informations__svg">
          <nuxt-icon name="arrow" filled />
        </div>
      </div>
    </a>
  </div>
</template>
<style lang="scss" scoped>
@import "Informations";
</style>
