<template>
  <div class="Parameters__main-container">
    <h2 class="Parameters__title">Parametry</h2>
    <div
      class="Parameters__row"
      v-for="(data, index) in parametersList"
      :key="data.label"
      :class="{ 'Parameters__row--gray': index % 2 === 0 }"
    >
      {{ index }}
      <div class="Parameters__label">{{ data.label }}</div>
      <div class="Parameters__text">{{ data.data }}</div>
    </div>
  </div>
</template>
<script setup>
const parametersList = ref([
  { label: "Stan", data: "Nowy" },
  { label: "Faktura", data: "Nie wystawiam faktury" },
  { label: "Rodzaj", data: "inny" },
  { label: "Producent", data: "Inna (TEVOUP)" },
  { label: "Model", data: "ACMER R10" },
  {
    label: "Waga produktu z opakowaniem jednostkowym",
    data: "1.5 kg",
  },
]);
const information = ref({
  cos: "oskar",
  siemanko: ["siemanko"],
  szczepan: { imie: "szczepan" },
});
</script>
<style lang="scss" scoped>
@import "Parameters";
</style>
