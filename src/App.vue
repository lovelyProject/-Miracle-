<template>
  <div class="main-wrapper">
    <div class="wrapper">
      <Header />
      <Main :slides="slides" />
      <Footer />
    </div>
    <!-- Облака в нижней части блока -->
    <img
      src="@/assets/image/cloud-bottom-middle.png"
      class="main-wrapper__item main-wrapper__item-1"
      alt=""
    />
    <img
      src="@/assets/image/cloud-bottom-middle.png"
      class="main-wrapper__item"
      alt=""
    />
    <img
      src="@/assets/image/cloud-bottom-middle.png"
      class="main-wrapper__item main-wrapper__item-2"
      alt=""
    />
  </div>
</template>
<script>
import Header from "@/components/v-header.vue";
import Main from "@/components/v-main.vue";
import Footer from "@/components/v-footer.vue";

export default {
  name: "vApp",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      //Имитация данных с API
      slides: [
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
      ],
    };
  },
};
</script>
<style lang="sass">
//импорт шрифтов
@import url(@/assets/main.css)
//reset styles
html
  font-size: 198%
*, ::after, ::before
  margin: 0
  padding: 0
  font-size: 1.6rem
  box-sizing: border-box
  text-decoration: none
  list-style: none
  color: #333
  font-family: Kinopoisk
  font-weight: 400
//
.main-wrapper
  background: url("@/assets/image/header-bg.jpg") center / cover no-repeat
  min-height: 100vh
  position: relative
  overflow: hidden
  &__item
    position: absolute
    bottom: 0%
    width: 96rem
    &-1
      width: 72rem
      left: 33%
    &-2
      right: -25%
      bottom: 0%
.wrapper
  margin: 0 auto
  position: relative
@media (max-width: 3800px)
  html
    font-size: 200%
@media (max-width: 3200px)
  html
    font-size: 148%
@media (max-width: 2600px)
  html
    font-size: 128%
@media (max-width: 2200px)
  html
    font-size: 90%
@media (max-width: 1900px)
  html
    font-size: 86%
@media (max-width: 1712px)
  html
    font-size: 82%
@media (max-width: 1621px)
  html
    font-size: 70%
@media (max-width: 1422px)
  html
    font-size: 60%
@media (max-width: 1200px)
  html
    font-size: 53%
@media (max-width: 1140px)
  html
    font-size: 50%
@media (max-width: 1050px)
  html
    font-size: 48%
@media (max-width: 950px)
  html
    font-size: 45%
@media (max-width: 900px)
  html
    font-size: 39%
@media (max-width: 760px)
  html
    font-size: 33%
@media (max-width: 669px)
  html
    font-size: 28%
@media (max-width: 565px)
  html
    font-size: 20%
@media (max-width: 470px)
  html
    font-size: 18%
</style>
