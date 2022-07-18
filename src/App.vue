<template>
  <div class="main__content">
    <header-block/>
    <main>
      <about-village/>
      <additional-description/>
      <infrastructure-block/>
      <speech-block/>
      <gen-plan/>
      <driving-directions/>
        <swiper
                :slidesPerView="4"
                :spaceBetween="5"
                :loop="true"
                :modules="modules"
                class="slider"
        >
          <swiper-slide
                  v-for="item in items"
                  :key="item.id"
          >
            <img :src="item.url"/>
          </swiper-slide>
        </swiper>
      <swiper
              :modules="modules"
              class="mobile__slider"
      >
        <swiper-slide
                v-for="item in items"
                :key="item.id"
        >
          <img class="mobile__image" :src="item.url"/>
        </swiper-slide>
      </swiper>
        <map-point/>
    </main>
    <footer-block/>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import 'swiper/swiper-bundle.css'
import HeaderBlock from './components/HeaderBlock.vue'
import AboutVillage from './components/AboutVillage.vue'
import AdditionalDescription from './components/AdditionalDescription.vue'
import InfrastructureBlock from './components/InfrastructureBlock.vue'
import SpeechBlock from './components/SpeechBlock.vue'
import GenPlan from "./components/GenPlan";
import DrivingDirections from "./components/DrivingDirections";
import FooterBlock from "./components/FooterBlock";
import MapPoint from "./components/MapPoint";

export default {
  name: 'App',
  components: {
      MapPoint,
      FooterBlock,
      DrivingDirections,
      GenPlan,
      HeaderBlock,
      AboutVillage,
      AdditionalDescription,
      InfrastructureBlock,
      SpeechBlock,
      Swiper,
      SwiperSlide,
  },
  data () {
      return {
          items: [
              {id: 0, url: '/static/One.jpeg'},
              {id: 1, url: '/static/Two.jpeg'},
              {id: 2, url: '/static/row1.png'},
              {id: 3, url: '/static/Four.jpeg'},
          ]
      }
  }

}
</script>

<style lang="sass">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap')
*
  box-sizing: border-box
  position: relative

  &::before, &::after
    box-sizing: border-box

ul[class], ol[class]
  padding: 0

body, h1, h2, h3, h4, p, ul[class], ol[class], li, figure, figcaption, blockquote, dl, dd
  margin: 0

body
  min-height: 100vh
  scroll-behavior: smooth
  text-rendering: optimizeSpeed
  line-height: 1.5

ul[class], ol[class]
  list-style: none

a:not([class])
  text-decoration-skip-ink: auto

img
  max-width: 100%
  display: block

article > * + *
  margin-top: 1em

input, button, textarea, select
  font: inherit

@media (prefers-reduced-motion: reduce)
  *
    animation-duration: 0.01ms !important
    animation-iteration-count: 1 !important
    transition-duration: 0.01ms !important
    scroll-behavior: auto !important
#app
  font-family: 'Montserrat', sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
.main__content
  display: flex
  flex-direction: column
  position: relative
.about__village__article__more
  display: flex
  flex-direction: row
  color: #6ED669
  gap: 18px
  p
    font-style: normal
    font-weight: 500
    font-size: 16px
    line-height: 18px
    letter-spacing: -0.01em
.slider
  height: 291px
.swiper-container
  width: 100%

.swiper-wrapper
  width: 50%

.swiper-slide
  padding: 0px
  width: auto
  margin-right: -30px !important

.my-gallery figure
  margin: 0px
.mobile__slider
  display: none
.main__swiper_left
@media screen and (max-width: 1024px)
  .slider
    display: none
  .mobile__slider
    display: block
  .swiper-wrapper
    width: min-content
  .swiper-slide
    padding: 24px 0px 24px 0px
    width: min-content
    text-align: center
    margin-right: 0px !important
    margin-left: 0px
  .swiper-slide:first-child
    padding: 24px 0px 24px 0px
    width: min-content
    text-align: center
    margin-right: 0px !important
    margin-left:  40px
  .mobile__image
  .mobile__image
    width: 80%
    height: 300px
</style>
