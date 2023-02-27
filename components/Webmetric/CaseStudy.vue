<template>
  <div class="CaseStudy__main-container">
    <div class="CaseStudy__center-container">
      <div class="CaseStudy__title-container">
        <span class="CaseStudy__title-span">Historie Sukcesów</span>
        <h3 class="CaseStudy__title-h3">Sprawdź nasze case study</h3>
      </div>
      <div class="CaseStudy__flex">
        <WebmetricCaseStudyBox
          v-for="data in caseStudyData"
          :key="data.title"
          :case-study-data="data"
          class="CaseStudy__box"
        />
        <WebmetricCaseStudyContact />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
interface CaseStudyData {
  srcLogo: string;
  srcImage: string;
  title: string;
  label: string;
  baranek?: string;
}
interface TakData {
  siemanko: number;
  oskar: boolean;
  nie: string;
}
const caseStudyData = ref<CaseStudyData[]>([
  {
    srcLogo: "casestudy-logo1",
    srcImage: "/assets/img/casestudy1.png",
    title: "Projekt UI/UX aplikacji webowej chatbota",
    label: "Aplikacje / Projektowanie UI",
    baranek: "oskar",
  },
  {
    srcLogo: "casestudy-logo2",
    srcImage: "/assets/img/casestudy2.png",
    title: "Projekt aplikacji dla uczelni wyższej ",
    label: "Aplikacje / Projektowanie UI",
  },
  {
    srcLogo: "casestudy-logo3",
    srcImage: "/assets/img/casestudy3.png",
    title: "Jak zwiększyć kowersję wersji demo aplikacji?",
    label: "Aplikacje / Badania UX",
  },
]);
const tak = ref<TakData>({
  siemanko: 12342,
  oskar: true,
  nie: "tak",
});
</script>
<style lang="scss" scoped>
@import "CaseStudy";
</style>
