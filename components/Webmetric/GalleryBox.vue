<template>
  <div class="GalleryBox__main-container">
    <div class="GalleryBox__dark-shadow"></div>
    <img :src="galleryBoxData.srcImage" class="GalleryBox__photo" />
    <div class="GalleryBox__title-container">
      <span
        class="GalleryBox__title"
        :style="{ color: galleryBoxData.color }"
        >{{ galleryBoxData.title }}</span
      >
      <p class="GalleryBox__information">
        Treść o projektowaniu użytecznych interfejsów
      </p>
    </div>
  </div>
</template>
<script setup>
defineProps({
  galleryBoxData: {
    required: true,
  },
});
</script>
<style lang="scss" scoped>
@import "GalleryBox";
</style>
