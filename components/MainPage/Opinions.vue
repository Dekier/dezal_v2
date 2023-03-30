<template>
  <div class="Opinions__main-container">
    <h2 class="Opinions__title">
      Zaufało nam już ponad 4100 osób w Poznaniu!
      <div class="Opinions__arrow-container">
        <button
          class="Opinions__arrow-left-button"
          :class="{ 'Opinions__arrow-active': isActiveButton }"
          @click="changeActiveButton()"
        >
          <img :src="rightArrowSrc()" class="Opinions__arrow" />
          <!-- <NuxtIcon
            name="Arrow_light"
            class="Opinions__arrow"
            filled
          ></NuxtIcon> -->
        </button>
        <button
          class="Opinions__arrow-right-button"
          :class="{ 'Opinions__arrow-active': isActiveButton }"
          @click="changeActiveButton()"
        >
          <img :src="rightArrowSrc()" class="Opinions__arrow" />
          <!-- <NuxtIcon
            name="Arrow_light"
            class="Opinions__arrow"
            filled
          ></NuxtIcon> -->
        </button>
      </div>
    </h2>
    <div class="Opinions__center-container">
      <div class="Opinions__links-container">
        <CommonGoogleOpinion
          v-for="data in googleOpinions"
          :key="data.name"
          :product-data="data"
        />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
interface GoogleOpinions {
  name: string;
  date: string;
  text: string;
  link: string;
  isActiveShowMore?: boolean;
}
const rightArrowSrc = () => {
  if (isActiveButton.value) {
    return "/_nuxt/assets/icons/Arrow_.svg";
  } else {
    return "/_nuxt/assets/icons/Arrow_light.svg";
  }
};
const isActiveButton = ref<boolean>(false);
const changeActiveButton = () => {
  isActiveButton.value = !isActiveButton.value;
};
const googleOpinions = ref<GoogleOpinions[]>([
  {
    name: "Monika",
    date: "Listopad 2022",
    text: "Już drugi raz jestem klientką firmy Deżal i oczywiście i tym razem się nie zawiodłam. Pełen profesjonalizm, szybka realizacja, fachowość i super doradztwo...",
    link: "https://g.co/kgs/bN3G8F",
    isActiveShowMore: true,
  },
  {
    name: "Michalina",
    date: "Luty 2023",
    text: "Super pomoc i responsywność. Rolety przygotowane oraz zamontowane w szybkim czasie i leżą jak ulał. Polecam.",
    link: "https://g.co/kgs/gR9LNe",
  },
  {
    name: "Sebastian",
    date: "Sierpień 2022",
    text: "Kontakt, obsługa i cena za świadczone usługi 5/5. Każdemu polecam, nie mam nic do zarzucenia. Cały montaż oraz zakup przeszedł bezproblemowo.",
    link: "https://g.co/kgs/7bCbCP",
  },
  {
    name: "Marcin",
    date: "Październik 2022",
    text: "Profesjonalne i szybkie wykonanie. Pan Dariusz jest zawsze skory do pomocy. Nowe rolety uratowały nas podczas ostatnich upałów ;)  Polecam każdemu!",
    link: "https://g.co/kgs/VS7AXq",
  },
  {
    name: "Maciej",
    date: "Marzec 2023",
    text: "Firma świadczy usługi na wysokim poziomie. Szybkie terminy realizacji. Świetna współpraca. Polecam.",
    link: "https://g.co/kgs/Kh3dsZ",
  },
  {
    name: "Joanna",
    date: "Listopad 2022",
    text: "Montaż rolet wykonany dokładnie i estetycznie. Termin dotrzymany. Dobry kontakt z klientem. Polecam.",
    link: "https://g.co/kgs/qK6ssq",
  },
  {
    name: "Patrycja",
    date: "Październik 2022",
    text: "Bardzo serdecznie polecam usługi firmy DEŻAL. Pan Dariusz jest świetnym fachowcem, wszystko przebiegło szybko, sprawnie i profesjonalnie 🙂.",
    link: "https://g.co/kgs/2ayqTy",
  },
  {
    name: "Krzysztof",
    date: "Luty 2022",
    text: "Kilka tygodni temu zostały u nas założone rolety w kasetkach. Wszystko działa pięknie. Tempo i jakość realizacji bez zarzutów, a sam kontakt z Właścicielem również należy pochwalić.",
    link: "https://g.co/kgs/7c6s9c",
    isActiveShowMore: true,
  },
  {
    name: "Konrad",
    date: "Kwiecień 2022",
    text: "Miałem zamówić rolety w innej firmie z której usług wcześniej korzystałem kilka razy, ale oferta wydawałsprawdzić w jeszcze jednym punkcie i na podstawie opinii wybrałem firmę DEŻAL...",
    link: "https://g.co/kgs/ZDxmVd",
    isActiveShowMore: true,
  },
  {
    name: "Małgorzata",
    date: "Czerwiec 2022",
    text: "Szybka realizacja, fachowe porady 👍Bardzo duży wybór materiałów oraz przystępna cena.Polecam.",
    link: "https://g.co/kgs/gUSP5T",
  },
]);
</script>
<style lang="scss" scoped>
@import "Opinions";
</style>
