<template>
  <div class="GoogleOpinion__main-container">
    <a :href="productData.link">
      <div class="GoogleOpinion__center-container">
        <div class="GoogleOpinion__title-container">
          <div class="GoogleOpinion__star-container">
            <NuxtIcon
              v-for="n in 5"
              :key="n"
              name="yellowstar"
              class="GoogleOpinion__star"
              filled
            />
          </div>

          <h3 class="GoogleOpinion__title">
            {{ productData.name }} | {{ productData.date }}
          </h3>
        </div>
        <p class="GoogleOpinion__text">
          {{ productData.text
          }}<span
            v-if="productData.isActiveShowMore"
            class="GoogleOpinion__show-more"
            >Czytaj więcej</span
          >
        </p>
        <p class="GoogleOpinion__opinion">
          Opinia z
          <NuxtIcon name="Googlelogo" filled class="GoogleOpinion__logo" />
        </p>
      </div>
    </a>
  </div>
</template>
<script setup lang="ts">
interface ProductData {
  name: string;
  date: string;
  text: string;
  link: string;
  isActiveShowMore?: boolean;
}
defineProps<{
  productData: ProductData;
}>();
</script>
<style lang="scss" scoped>
@import "GoogleOpinion";
</style>
