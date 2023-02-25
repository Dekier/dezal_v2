<template>
  <div
    class="FaqBox__box-container"
    :class="{ 'FaqBox__box-container--active': isActiveButton }"
  >
    <div
      class="FaqBox__line"
      :class="{ 'FaqBox__line--active': isActiveButton }"
    ></div>
    <button class="FaqBox__button" @click="changeActiveButton()">
      <span> {{ faqData.title }}</span>
      <nuxt-icon
        name="arrow"
        filled
        class="FaqBox__icon"
        :class="{ 'FaqBox__icon--active': isActiveButton }"
      />
    </button>
    <div
      class="FaqBox__box-hidden"
      :class="{ 'FaqBox__box-hidden--active': isActiveButton }"
    >
      <p class="FaqBox__margin">
        {{ faqData.label }}
      </p>
      <p>
        {{ faqData.label2 }}
      </p>
      <div class="FaqBox__link-container">
        <nuxt-link to="/kontakt" class="FaqBox__link">ZOBACZ WIECEJ</nuxt-link>
      </div>
    </div>
  </div>
</template>
<script setup>
const isActiveButton = ref(false);
const changeActiveButton = () => {
  isActiveButton.value = !isActiveButton.value;
};
defineProps({
  faqData: {
    required: true,
  },
});
</script>
<style lang="scss" scoped>
@import "FaqBox";
</style>
