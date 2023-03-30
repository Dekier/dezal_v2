<template>
  <div
    class="ProductBox__main-container"
    :class="setMainContainerClass('ProductBox__main-container')"
  >
    <div
      class="ProductBox__square"
      :class="setSquareClass('ProductBox__square')"
    ></div>
    <div class="ProductBox__image-container">
      <div v-if="productData.isActiveStar" class="ProductBox__star-container">
        <nuxt-icon name="star" filled class="ProductBox__star" />
        <span class="ProductBox__star-text">Najczęściej wybierane</span>
      </div>
      <img
        :src="productData.imgSrc"
        class="ProductBox__image"
        :class="setImageClass('ProductBox__image')"
      />
    </div>
    <div class="ProductBox__title">{{ productData.title }}</div>
    <div class="ProductBox__text" :class="setTextClass('ProductBox__text')">
      {{ productData.text }}
    </div>
    <CommonButtonArrow :path="productData.path" text="czytaj więcej" />
  </div>
</template>
<script setup lang="ts">
interface ProductData {
  title: string;
  imgSrc: string;
  text: string;
  path: string;
  isActiveStar?: boolean;
  typeStyle?: string;
}
const props = defineProps<{
  productData: ProductData;
}>();

const setImageClass = (defaultClass: string) => {
  if (!props.productData.typeStyle) return;
  switch (props.productData.typeStyle) {
    case "image-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
    case "image-height-width-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
    case "image-long-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
    case "image-short-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;

    default:
      break;
  }
};
const setTextClass = (defaultClass: string) => {
  if (!props.productData.typeStyle) return;
  switch (props.productData.typeStyle) {
    case "image-height-width-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
    case "image-long-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;

    default:
      break;
  }
};
const setMainContainerClass = (defaultClass: string) => {
  if (!props.productData.typeStyle) return;
  switch (props.productData.typeStyle) {
    case "image-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
  }
};
const setSquareClass = (defaultClass: string) => {
  if (!props.productData.typeStyle) return;
  switch (props.productData.typeStyle) {
    case "image-long-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
    case "image-short-height-fit":
      return `${defaultClass}--${props.productData.typeStyle}`;
  }
};
</script>
<style lang="scss" scoped>
@import "ProductBox";
</style>
