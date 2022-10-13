<template>
  <swiper :modules="modules" :slides-per-view="1" :navigation="swiperOption.navigation" @reach-end="onSwiperEnd" @reach-beginning="onSwiperBegin">
    <swiper-slide>
      <div>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident distinctio exercitationem iste. Alias, enim. Nemo voluptas aut sint corporis id?</p>
        <h3>Rohan Rohiyan</h3>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos ipsam totam obcaecati laudantium reiciendis dolore perferendis ratione! Quis ut deleniti quaerat reprehenderit pariatur aspernatur asperiores fugit, eaque officia,
          velit, dignissimos reiciendis?
        </p>
        <h3>Rendi Rendulan</h3>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perspiciatis voluptas tenetur omnis laborum quibusdam nihil soluta a quaerat?</p>
        <h3>Sepuh Sependi</h3>
      </div>
    </swiper-slide>
    <swiper-slide>
      <div>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Provident distinctio exercitationem iste. Alias, enim. Nemo voluptas aut sint corporis id?</p>
        <h3>Raden Rombong Rapangsit</h3>
      </div>
    </swiper-slide>
  </swiper>
</template>
<script>
import { Navigation } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
import 'swiper/css/bundle'
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiperEnd = () => {
      document.querySelector('button.swiper-next').classList.remove('swiperButton')
      document.querySelector('button.swiper-prev').classList.add('swiperButton')
    }
    const onSwiperBegin = () => {
      document.querySelector('button.swiper-next').classList.add('swiperButton')
      document.querySelector('button.swiper-prev').classList.remove('swiperButton')
    }
    const swiperOption = {
      navigation: { nextEl: '.swiper-next', prevEl: '.swiper-prev' },
      autoplay: {
        delay: 5000,
        disableOnInteraction: false,
      },
    }
    return {
      modules: [Navigation],
      swiperOption,
      onSwiperEnd,
      onSwiperBegin,
    }
  },
}
</script>
