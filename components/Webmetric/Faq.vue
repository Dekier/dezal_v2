<template>
  <div class="Faq__main-container">
    <div class="Faq__center-container">
      <div class="Faq__title-container">
        <span class="Faq__subtitle">FAQ</span>
        <h3 class="Faq__title">Najczęściej zadawane pytania</h3>
      </div>
      <WebmetricFaqBox
        v-for="data in faqData"
        :key="data.title"
        :faq-data="data"
      />
    </div>
  </div>
</template>
<script setup>
const faqData = ref([
  {
    title: "Czym wyróżnia się nasza agencja UX?",
    label:
      "Jako agencja UX łączymy autorsko 3 obszary:– projektowanie UI/UX,– badań z użytkownikami,– analityką internetową",
    label2:
      "Poprzez takie połączenie opiekujemy się i wytwarzamy najlepsze interfejsy użytkownika dla produktów cyfrowych. Dzięki temu są one bardziej użyteczne i sprzedają więcej.Posiadamy ponad 10-letnie doświadczenie w kreowaniu i optymalizacji produktów cyfrowych. Łączymy podejście analizy ilościowej i badań jakościowych UX.",
  },
  {
    title: "Co to jest User Experience",
    label:
      "User Experience (UX) to całość doświadczeń użytkownika pojawiających się podczas korzystania z usług, produktów oraz interfejsów.",
    label2:
      "Dla naszej agencji UX jest to poznawanie i projektowanie doświadczeń użytkownika, czyli, nadawanie wartości Twojemu produktowi cyfrowemu. Sprawienie, by odpowiadał na potrzeby klientów i rozwiązywał ich realne problemy. Lepsze doświadczenia sprzedają więcej.",
  },
]);
</script>
<style lang="scss" scoped>
@import "Faq";
</style>
