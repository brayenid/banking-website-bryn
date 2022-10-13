<script setup>
import Button from './Button.vue'
</script>
<template>
  <div class="service">
    <div class="flex flex-col xl:flex-row xl:justify-around xl:items-center">
      <div class="servImg">
        <img src="@/img/service/Image.png" alt="" />
      </div>
      <div class="serDet">
        <h1 class="font-bold">Boost Productivity</h1>
        <p class="text-gray-700 max-w-md my-7 leading-8">Ciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.Ciatis unde omnis iste natus error sit.</p>
        <Button content="Get Started" />
      </div>
    </div>
    <div class="flex flex-col items-end xl:flex-row-reverse xl:justify-around xl:items-center mt-36">
      <div class="servImg">
        <img src="@/img/service/1.png" alt="" />
      </div>
      <div class="serDet text-right xl:text-left">
        <h1 class="font-bold">Highest Output</h1>
        <p class="text-gray-700 max-w-md my-7 leading-8">Ciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.Ciatis unde omnis iste natus error sit.</p>
        <Button content="Get Started" />
      </div>
    </div>
  </div>
</template>
<style scoped>
.serDet {
  font-size: calc(14px + 0.3vw);
}
.serDet h1 {
  font-size: calc(18px + 1vw);
}
</style>
