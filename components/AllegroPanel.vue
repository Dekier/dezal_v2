<template>
  <div class="AllegroPanel__main-container">
    <div class="AllegroPanel__left-container">
      <AllegroPanelParameters />
      <AllegroPanelDescription />
      <AllegroPanelOpinions />
    </div>
    <div class="AllegroPanel__sticky-container">
      <div class="AllegroPanel__right-container">
        <AllegroPanelPayments />
        <AllegroPanelInformations />
        <AllegroPanelLinks />
      </div>
    </div>
  </div>
</template>
<script setup>
const count = ref(0);
</script>
<style lang="scss" scoped>
@import "AllegroPanel";
</style>
