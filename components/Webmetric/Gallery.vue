<template>
  <div class="Gallery__main-container">
    <div class="Gallery__center-container">
      <div class="Gallery__title-container">
        <span class="Gallery__subtitle">DOWIEDZ SIĘ WIĘCEJ</span>
        <h3 class="Gallery__title">Wiedza o UX/UI/CRO</h3>
      </div>
      <div class="Gallery__row">
        <WebmetricGalleryBox
          v-for="data in galleryBoxData"
          :key="data.title"
          :gallery-box-data="data"
        />
      </div>
    </div>
  </div>
</template>
<script setup>
const galleryBoxData = ref([
  {
    srcImage: "/assets/img/Gallery1.jpg",
    title: "UX/UI DESIGN",
    label: "Treści o projektowaniu użytecznych interfejsów",
    color: "#46FEDA",
  },
  {
    srcImage: "/assets/img/Gallery2.png",
    title: "BADANIA UX",
    label: "Artykuły o badaniach UX i wykorzystyaniu ich w biznesie",
    color: "#7946FB",
  },
  {
    srcImage: "/assets/img/Gallery3.png",
    title: "Analityka",
    label: "Wpisy o optymalizacji konwersji",
    color: "#FF0098",
  },
]);
</script>
<style lang="scss" scoped>
@import "Gallery";
</style>
