<template>
  <NuxtLink to="/rolety" class="CaseStudyBox__link">
    <div class="CaseStudyBox__item-container">
      <div class="CaseStudyBox__item-data">
        <div class="CaseStudyBox__item-logo">
          <NuxtIcon
            :name="caseStudyData.srcLogo"
            class="CaseStudyBox__svg"
          ></NuxtIcon>
        </div>
        <div class="CaseStudyBox__item-categories">
          <span class="CaseStudyBox__item-subtitle"
            >{{ caseStudyData.label }}
          </span>
          <span class="CaseStudyBox__item-subtitle"></span>
        </div>
        <div class="CaseStudyBox__item-title-container">
          <h5 class="CaseStudyBox__item-title">{{ caseStudyData.title }}</h5>
        </div>
      </div>
      <div class="CaseStudyBox__image-container">
        <img
          :src="caseStudyData.srcImage"
          alt="czater"
          class="CaseStudyBox__item-img"
        />
      </div>
    </div>
  </NuxtLink>
</template>
<script setup>
defineProps({
  caseStudyData: {
    required: true,
  },
});
</script>
<style lang="scss" scoped>
@import "CaseStudyBox";
</style>
