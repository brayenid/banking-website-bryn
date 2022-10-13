<script setup>
import Button from './Button.vue'
</script>
<template>
  <header class="font-Poppins pb-4">
    <div class="lg:flex justify-center py-14 items-center md:px-14 box-border gap-4">
      <div class="bigImg flex-1 order-2 mb-10">
        <img class="w-full rounded-[2.9rem] shadow-md" src="@/img/header/Image.png" alt="" />
      </div>
      <div class="bigTitle flex-1 order-1">
        <h1 class="font-bold drop-shadow-sm">Every transaction is special for us.</h1>
        <p class="text-base leading-8 my-5 text-gray-700">Aiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudan.</p>
        <Button content="Get Started" />
      </div>
    </div>
    <div class="corpsLogo">
      <ul class="corpsList">
        <li><img src="@/img/header/apple.png" alt="" /></li>
        <li><img src="@/img/header/adobe.png" alt="" /></li>
        <li><img src="@/img/header/slack.png" alt="" /></li>
        <li><img src="@/img/header/spotify.png" alt="" /></li>
        <li><img src="@/img/header/google.png" alt="" /></li>
      </ul>
    </div>
  </header>
</template>
