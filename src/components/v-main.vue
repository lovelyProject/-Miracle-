<template>
  <main class="main">
    <div class="main__logo">
      <img class="main__logo-item" src="@/assets/image/logo.png" alt="cloud" />
    </div>
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
</template>

<script>
import Carousel from "@/components/carousel/v-carousel.vue";
export default {
  name: "vMain",
  props: ["slides"],
  components: {
    Carousel,
  },
};
</script>
<style lang="sass">
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
</style>
