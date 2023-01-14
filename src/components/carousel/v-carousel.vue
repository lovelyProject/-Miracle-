<template>
  <div class="v-carousel">
    <div class="v-carousel__counter">
      <span class="counter bold">{{ currentSlide + 1 }}/8</span>
    </div>
    <div class="v-carousel__content">
      <vCarouselItem
        v-for="(slide, index) in slides"
        :key="index"
        :slide="slide"
        :currentSlide="currentSlide"
        :index="index"
        :direction="direction"
      />
    </div>
    <button
      v-show="currentSlide != 0"
      class="carousel-control prev-slide"
      @click="prevSlide"
    >
      <svg viewBox="0 0 17 5" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0.963876 2.38841L16.1642 2.38841" stroke="#333333" />
        <path
          d="M14.4482 4.08231L16.1689 2.3616L14.4482 0.670764"
          stroke="#333333"
        />
      </svg>
    </button>
    <button
      class="carousel-control next-slide"
      @click="nextSlide"
      v-show="currentSlide != 7"
    >
      <svg viewBox="0 0 17 5" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0.963876 2.38841L16.1642 2.38841" stroke="#333333" />
        <path
          d="M14.4482 4.08231L16.1689 2.3616L14.4482 0.670764"
          stroke="#333333"
        />
      </svg>
    </button>
  </div>
</template>

<script>
import vCarouselItem from "@/components/carousel/v-carousel-item.vue";
export default {
  components: {
    vCarouselItem,
  },
  props: ["slides"],
  data() {
    return {
      currentSlide: 0,
      direction: "",
    };
  },
  methods: {
    nextSlide() {
      this.currentSlide++;
      this.direction = "right";
    },
    prevSlide() {
      this.currentSlide--;
      this.direction = "left";
    },
  },
};
</script>

<style lang="sass">
.v-carousel
  margin: 0 auto
  max-width: 90rem
  position: relative
  overflow: hidden
  min-height: 50rem
  &__counter
    position: absolute
    left: 49%
    width: 5.6rem
    height: 5.6rem
    background-color: #fff
    margin: 0 auto
    border-radius: 50%
    display: flex
    align-items: center
    justify-content: center
    box-shadow: 0 .5rem 2.6rem rgba(0, 0, 0, 0.1)
    margin-bottom: 2rem
    & .counter
      font-size: 1.5rem
    &__content
      margin-top: 7rem
      position: relative
.btn-arrow
  width: 2.8rem
  height: .5rem
.carousel-control
  border: .1rem solid rgba(51,51,51,1)
  border-radius: 50%
  width: 4rem
  height: 4rem
  position: absolute
  cursor: pointer
  z-index: 2
  display: flex
  justify-content: center
  align-items: center
  background-color: rgba(255,255,255,1)
  & svg
    width: 1.7rem
    height: .5rem
  &:hover
    background-color: #fff
.prev-slide
  top: 50%
  transform: rotate(180deg)
.next-slide
  top: 50%
  right: 0
</style>
