<template>
  <nuxt-link :to="path" class="ButtonArrow__main-container">
    <div class="ButtonArrow__center-container">
      <span v-if="text" class="ButtonArrow__text">{{ text }}</span>
      <div class="ButtonArrow__square">
        <nuxt-icon name="ArrowRight" filled class="ButtonArrow__arrow" />
      </div>
    </div>
    <div class="ButtonArrow__line"></div>
  </nuxt-link>
</template>
<script setup lang="ts">
defineProps<{
  path: string;
  text?: string;
}>();
</script>
<style lang="scss" scoped>
@import "ButtonArrow";
</style>
