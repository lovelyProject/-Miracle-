<template>
  <transition :name="direction" mode="in-out">
    <div class="v-carousel-item" v-show="index === currentSlide">
      <img
        class="v-carousel-item__photo"
        src="@/assets/slides/racer.png"
        alt=""
      />
      <p class="v-carousel-item__text">{{ slide.text }}</p>
    </div>
  </transition>
</template>

<script>
export default {
  props: ["slide", "currentSlide", "index", "direction"],
};
</script>

<style lang="sass">
.v-carousel-item
    position: absolute
    top: 0
    left: 0
    right: 0
    bottom: 0
    display: flex
    flex-direction: column
    justify-content: flex-end
    &__text
        max-width: 80rem
        display: flex
        flex-wrap: wrap
        margin: 27rem auto 0 auto
        font-size: 2rem
        line-height: 3.2rem
        letter-spacing: 0.4px
        position: relative
        font-weight: 500
        z-index: 4
        margin-bottom: 2rem
    &__photo
        width: 40%
        position: absolute
        left: 30%
        top: 15%
.right-enter-active
    animation: rightInAnimation .5s ease-in-out
.right-leave-active
    animation: rightOutAnimation .5s ease-in-out
@keyframes rightInAnimation
    from
        transform: translateX(100%)
    to
        transform: translateX(0)

@keyframes rightOutAnimation
    from
        transform: translateX(0)
    to
        transform: translateX(-100%)
.left-enter-active
    animation: leftInAnimation .4s ease-in-out
.left-leave-active
    animation: leftOutAnimation .4s ease-in-out
@keyframes leftInAnimation
    from
        transform: translateX(-100%)
    to
        transform: translateX(0)

@keyframes leftOutAnimation
    from
        transform: translateX(0)
    to
        transform: translateX(100%)
</style>
