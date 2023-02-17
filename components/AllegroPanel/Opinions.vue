<template>
  <div class="Opinions__main-container">
    <h2 class="Opinions__title">Opinie o produkcie</h2>
    <div class="Opinions__opinions-container">
      <div class="Opinions__score-container">
        <div class="Opinions__left">
          <p class="Opinions__name">Rewelacyjny</p>
          <div class="Opinions__rating">
            <div class="Opinions__row">
              <span>5,00</span>
              <span class="Opinions__small-number">/5</span>
            </div>
            <span class="Opinions__small-span">1 ocena</span>
          </div>
        </div>
        <div class="Opinions__right">
          <button class="Opinions__button" type="button">
            5 <nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="full-star" filled />
            <div class="Opinions__line--full"></div>
            <span class="Opinions__number">1</span>
          </button>
          <button class="Opinions__button" type="button">
            4 <nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="empty-star" filled />
            <div class="Opinions__line"></div>
            <span class="Opinions__number">0</span>
          </button>
          <button class="Opinions__button" type="button">
            3 <nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="full-star" filled /><nuxt-icon
              name="empty-star"
              filled
            /><nuxt-icon name="empty-star" filled />
            <div class="Opinions__line"></div>
            <span class="Opinions__number">0</span>
          </button>
          <button class="Opinions__button" type="button">
            2 <nuxt-icon name="full-star" filled /><nuxt-icon
              name="full-star"
              filled
            /><nuxt-icon name="empty-star" filled /><nuxt-icon
              name="empty-star"
              filled
            /><nuxt-icon name="empty-star" filled />
            <div class="Opinions__line"></div>
            <span class="Opinions__number">0</span>
          </button>
          <button class="Opinions__button" type="button">
            1 <nuxt-icon name="full-star" filled /><nuxt-icon
              name="empty-star"
              filled
            /><nuxt-icon name="empty-star" filled /><nuxt-icon
              name="empty-star"
              filled
            /><nuxt-icon name="empty-star" filled />
            <div class="Opinions__line"></div>
            <span class="Opinions__number">0</span>
          </button>
        </div>
      </div>
      <div class="Opinions__informations-container">
        <div class="Opinions__informations">
          <nuxt-icon name="positiv" class="Opinions__svg-positiv" filled />
          <p class="Opinions__paragraph">
            Opinie wystawiane sa po zakupie dla produktów od różnych
            sprzedających
          </p>
        </div>
        <a class="Opinions__link" href="faraway">Jak działają opinie?</a>
      </div>
    </div>
    <div class="Opinions__review-container">
      <h3 class="Opinions__review-title">Produkt nie ma jeszcze recenzji</h3>
      <p class="Opinions__review-text">Po zakupie opisz swoje wrażenia.</p>
      <p class="Opinions__review-text">
        Twoja recenzja pojawi się w tym miejscu i pomoże innym w podjęciu
        decyzji.
      </p>
    </div>
  </div>
</template>
<style lang="scss" scoped>
@import "Opinions";
</style>
