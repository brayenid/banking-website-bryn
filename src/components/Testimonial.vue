<script setup>
import Swiper from './Swiper.vue'
import NavigationSwiper from './NavigationSwiper.vue'
</script>
<template>
  <div class="testimonial">
    <div class="testimonialContent">
      <h1>Trusted by Agencies & Store Owners</h1>
      <div class="testimonialParagraph relative">
        <div class="relative z-20">
          <Swiper />
        </div>
        <div class="quote"><img class="w-32" src="@/img/testimonial/2ticks.svg" alt="" /></div>
      </div>
    </div>
    <div class="backgroundSection w-full absolute top-0 z-10">
      <div class="faceRow justify-around">
        <img src="@/img/testimonial/1.png" alt="" />
        <img src="@/img/testimonial/2.png" alt="" />
      </div>
      <div class="faceRow justify-between">
        <img src="@/img/testimonial/3.png" alt="" />
        <img src="@/img/testimonial/4.png" alt="" />
      </div>
      <div class="faceRow justify-around">
        <img class="faceRowImgLastLeft" src="@/img/testimonial/5.png" alt="" />
        <img class="faceRowImgLastRight" src="@/img/testimonial/6.png" alt="" />
      </div>
    </div>
    <div class="dotted">
      <div class="flex dotBlue h-[100%] items-end translate-y-8">
        <img src="@/img/testimonial/dottedbgBlue.png" alt="" />
      </div>
      <div class="flex dotRed h-[100%] items-start translate-y-52">
        <img src="@/img/testimonial/dottedbgRed.png" alt="" />
      </div>
    </div>
    <NavigationSwiper />
  </div>
</template>
<style scoped>
.faceRowImgLastLeft {
  transform: translateX(-8rem);
}
.faceRowImgLastRight {
  transform: translateX(8rem);
}
</style>
