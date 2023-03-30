<template>
  <div class="SectionProducts__main-container">
    <h2 class="SectionProducts__title">Jakich rolet potrzebujesz?</h2>
    <div class="SectionProducts__center-container">
      <div class="SectionProducts__left-panel">
        <CommonProductBox
          v-for="data in leftPanelData"
          :key="data.title"
          :product-data="data"
        />
      </div>
      <div class="SectionProducts__right-panel">
        <CommonProductBox
          v-for="data in rightPanelData"
          :key="data.title"
          :product-data="data"
        />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
interface LeftPanelData {
  title: string;
  imgSrc: string;
  text: string;
  path: string;
  isActiveStar?: boolean;
  typeStyle?: string;
  textStyle?: string;
  mainContainerStyle?: string;
  squareStyle?: string;
}
const leftPanelData = ref<LeftPanelData[]>([
  {
    title: "Plisy",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/plisy",
    isActiveStar: true,
  },
  {
    title: "Rolety Rzymskie",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/rzymskie",
    typeStyle: "image-long-height-fit",
  },
  {
    title: "Verticale",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/verticale",
    typeStyle: "image-height-width-fit",
  },
]);
interface RightPanelData {
  title: string;
  imgSrc: string;
  text: string;
  path: string;
  isActiveStar?: boolean;
  typeStyle?: string;
  textStyle?: string;
  mainContainerStyle?: string;
  squareStyle?: string;
}
const rightPanelData = ref<RightPanelData[]>([
  {
    title: "Rolety materiałowe",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/materialowe",
    typeStyle: "image-height-fit",
  },
  {
    title: "Rolety dzień-noc",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/dzien-noc",
    typeStyle: "image-height-width-fit",
  },
  {
    title: "Żaluzje",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/zaluzje",
    typeStyle: "image-height-fit",
  },
  {
    title: "Moskitiery",
    text: "to jedna z ciekawszych propozycji w systemach przeciwsłonecznych pod względem funkcjonalności. Bogata oferta tkanin spełni każde oczekiwania pod kątem zarówno dekoracyjności jak i stopnia zaciemnienia.",
    imgSrc: "/assets/img/product.png",
    path: "/moskitiery",
    typeStyle: "image-short-height-fit",
  },
]);
</script>
<style lang="scss" scoped>
@import "SectionProducts";
</style>
