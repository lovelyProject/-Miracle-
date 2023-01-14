<template>
  <div class="main-wrapper">
    <div class="wrapper">
      <header class="header">
        <div class="header__burger">
          <svg
            viewBox="0 0 22 17"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M1.47498 0.528625V0.0286255H0.974976V0.528625H1.47498ZM21.0958 0.528625H21.5958V0.0286255H21.0958V0.528625ZM21.0958 2.52863V3.02863H21.5958V2.52863H21.0958ZM1.47498 2.52863H0.974976V3.02863H1.47498V2.52863ZM1.47498 7.70923V7.20923H0.974976V7.70923H1.47498ZM21.0958 7.70923H21.5958V7.20923H21.0958V7.70923ZM21.0958 9.70923V10.2092H21.5958V9.70923H21.0958ZM1.47498 9.70923H0.974976V10.2092H1.47498V9.70923ZM1.47498 14.5V14H0.974976V14.5H1.47498ZM1.47498 16.5H0.974976V17H1.47498V16.5ZM21.0958 16.5V17H21.5958V16.5H21.0958ZM21.0958 14.5H21.5958V14H21.0958V14.5ZM1.97498 0.0286255H1.47498V1.02863H1.97498V0.0286255ZM20.5958 0.0286255H1.97498V1.02863H20.5958V0.0286255ZM21.0958 0.0286255H20.5958V1.02863H21.0958V0.0286255ZM21.5958 1.02863V0.528625H20.5958V1.02863H21.5958ZM21.5958 2.02863V1.02863H20.5958V2.02863H21.5958ZM21.5958 2.52863V2.02863H20.5958V2.52863H21.5958ZM20.5958 3.02863H21.0958V2.02863H20.5958V3.02863ZM1.97498 3.02863H20.5958V2.02863H1.97498V3.02863ZM1.47498 3.02863H1.97498V2.02863H1.47498V3.02863ZM0.974976 2.02863V2.52863H1.97498V2.02863H0.974976ZM0.974976 1.02863V2.02863H1.97498V1.02863H0.974976ZM0.974976 0.528625V1.02863H1.97498V0.528625H0.974976ZM1.97498 7.20923H1.47498V8.20923H1.97498V7.20923ZM20.5958 7.20923H1.97498V8.20923H20.5958V7.20923ZM21.0958 7.20923H20.5958V8.20923H21.0958V7.20923ZM21.5958 8.20923V7.70923H20.5958V8.20923H21.5958ZM21.5958 9.20923V8.20923H20.5958V9.20923H21.5958ZM21.5958 9.70923V9.20923H20.5958V9.70923H21.5958ZM20.5958 10.2092H21.0958V9.20923H20.5958V10.2092ZM1.97498 10.2092H20.5958V9.20923H1.97498V10.2092ZM1.47498 10.2092H1.97498V9.20923H1.47498V10.2092ZM0.974976 9.20923V9.70923H1.97498V9.20923H0.974976ZM0.974976 8.20923V9.20923H1.97498V8.20923H0.974976ZM0.974976 7.70923V8.20923H1.97498V7.70923H0.974976ZM1.47498 15H1.97498V14H1.47498V15ZM1.97498 15V14.5H0.974976V15H1.97498ZM1.97498 16V15H0.974976V16H1.97498ZM1.97498 16.5V16H0.974976V16.5H1.97498ZM1.97498 16H1.47498V17H1.97498V16ZM20.5958 16H1.97498V17H20.5958V16ZM21.0958 16H20.5958V17H21.0958V16ZM20.5958 16V16.5H21.5958V16H20.5958ZM20.5958 15V16H21.5958V15H20.5958ZM20.5958 14.5V15H21.5958V14.5H20.5958ZM20.5958 15H21.0958V14H20.5958V15ZM1.97498 15H20.5958V14H1.97498V15Z"
              fill="#333333"
            />
          </svg>
        </div>
        <nav class="header__vertical-menu">
          <ol class="header__vertical-menu-list">
            <li class="vertical-menu-list__item"></li>
            <li class="vertical-menu-list__item"></li>
            <li class="vertical-menu-list__item">
              <span class="bold item-number">03 </span> <span>Подсказки</span>
            </li>
            <li class="vertical-menu-list__item"></li>
          </ol>
        </nav>
        <div class="header__info">
          <span class="header__info-item">Скрольте вниз</span>
          <svg
            class="header__info-item"
            viewBox="0 0 6 64"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M3.03528 0.5V62.635" stroke="#333333" />
            <path
              d="M1.34137 60.9189L3.06208 62.6397L4.75292 60.9189"
              stroke="#333333"
            />
          </svg>
        </div>
      </header>
      <main class="main">
        <div class="main__logo">
          <img
            class="main__logo-item"
            src="@/assets/image/logo.png"
            alt="cloud"
          />
        </div>
        <div class="main__title-container"></div>
        <h1 class="main__title">ОНИ ДОЛЖНЫ ЧТО-ТО ЗНАТЬ</h1>
        <div class="main__content">
          <Carousel :slides="slides" />
          <div class="main__btn">
            <button href="#" class="main__btn-item">
              <span class="v-carousel__btn-text">Искать промокод</span>
              <svg
                class="btn-arrow"
                viewBox="0 0 28 5"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path d="M0.370911 2.8553L26.7406 2.8553" stroke="#333333" />
                <path
                  d="M25.0246 4.54921L26.7453 2.8285L25.0246 1.13766"
                  stroke="#333333"
                />
              </svg>
            </button>
          </div>
        </div>
      </main>
      <footer class="footer">
        <div class="footer-container">
          <span class="footer__link">hd.kinopoisk.ru</span>
        </div>
      </footer>
    </div>
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
import Carousel from "./components/carousel/v-carousel.vue";

export default {
  name: "vApp",
  components: {
    Carousel,
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
.header
  display: flex
  flex-direction: column
  justify-content: space-between
  position: fixed
  height: 100vh
  z-index: 1
  padding: 2rem 0 0 2rem
  &__vertical-menu-list
    display: inline-flex
    flex-direction: column
  &__info
    display: flex
    flex-direction: column
    align-items: center
    width: 2.1rem
    margin-left: -.7rem
    margin-bottom: 3rem
    font-size: 2rem
    & svg
      display: block
      height: 6.4rem
      padding-top: 1rem
    & span
      display: block
      font-size: 1.4rem
      writing-mode: vertical-rl
      transform: rotate(180deg)
  &__slider
    width: 12.2rem
    height: 16.1rem
    & img
      width: 100%
  &__burger
    width: 2rem
    height: 1.6rem
    cursor: pointer
.vertical-menu-list__item
  min-width: .7rem
  position: relative
  display: inline
  white-space: nowrap
  &:empty
    display: inline-block
    max-width: .8rem
  &::after
    content: ""
    position: absolute
    width: 100%
    left: 0
    height: .1rem
    background-color: #333
    top: 120%
  &:not(:last-child)
    margin-bottom: 4rem
.item-number
  margin-right: 2rem
.bold
  font-weight: 600
  color: #2E332A
.main
  text-align: center
  display: flex
  flex-direction: column
  justify-content: space-between
  min-height: 100vh
  position: relative
  &__btn
    padding-bottom: 4rem
    &-item
      position: relative
      margin: 0 auto
      display: flex
      align-items: center
      border: none
      cursor: pointer
      background-color: #fff
      text-decoration: none
      color: #333333
      padding: 2rem 3.2rem 2rem
      box-shadow: 0 .5rem 2.6rem rgba(11, 75, 92, 0.0975713)
      border-radius: .8rem
      align-items: center
      z-index: 6
      &:hover
        background-color: rgba(0,0,0,0.1)
      & span
        margin-right: 2rem
  &__items
    padding-bottom: 2rem
    position: relative
    overflow: hidden
    z-index: 0
  &__content
    position: relative
  &__logo
    position: relative
    padding-top: 2rem
    background: linear-gradient(0deg, rgba(255, 255, 255, 0.0001) 7.86%, #FFFFFF 82.86%)
    &-item
      width: 18.2rem
      margin-bottom: 2.4rem
  &__title
    font-weight: 700
    font-size: 4.5rem
    line-height: 7.2rem
    text-transform: uppercase
    color: #FFCC64
    position: relative
    z-index: 1
    font-family: Futura
.footer
  position: fixed
  top: calc(50% - 1rem)
  right: 0
  margin-right: 3rem
  z-index: 6
  &-container
  &__link
    writing-mode: vertical-lr
    transform: rotate(0deg)
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
    font-size: 98%
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
