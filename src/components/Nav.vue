<script setup>
import { RouterLink } from 'vue-router'
import Person from '../icons/Person.vue'
import Hamburger from './Hamburger.vue'

const modalSign = function () {
  document.querySelector('.modalSign').classList.toggle('showModal')
}
document.addEventListener('click', (e) => {
  if (!e.target.closest('.modalSign') && !e.target.closest('.signin') && document.querySelector('.modalSign').classList.contains('showModal')) {
    document.querySelector('.modalSign').classList.remove('showModal')
  }
  if (!e.target.closest('.menuList') && !e.target.closest('.hamburgerBtn') && document.querySelector('.menuList').classList.contains('showMenu')) {
    document.querySelector('.hamCheck').click()
  }
})

const showMenu = () => {
  document.querySelector('.menuList').classList.toggle('showMenu')
}
</script>
<template>
  <nav class="font-Poppins flex justify-between items-center">
    <div class="logo order-3 sm:order-none">
      <img src="../../img/header/logo.png" alt="" />
    </div>
    <Hamburger @click="showMenu" class="hamburgerBtn order-1 sm:order-none relative z-50" />
    <ul class="menuList">
      <li><RouterLink active-class="active" to="/">Home</RouterLink></li>
      <li><RouterLink active-class="active" to="/feature">Features</RouterLink></li>
      <li><RouterLink active-class="active" to="/showcase">Showcase</RouterLink></li>
      <li><RouterLink active-class="active" to="/pricing">Pricing</RouterLink></li>
    </ul>
    <div class="signin order-4 sm:order-none">
      <button @click="modalSign">
        <Person />
      </button>
      <div class="hidden modalSign text-center bg-slate-100 px-6 pt-12 pb-6 rounded-lg absolute right-10 top-24 shadow-lg max-w-sm">
        <p class="mb-5">Don't have an account?</p>
        <button class="bg-blue-600 text-white px-5 py-2 rounded-lg hover:bg-white border border-blue-600 transition-all hover:text-blue-600 mb-8">Sign Up</button>
        <p class="text-xs">If you already have an account, please <a href="#" class="font-bold hover:text-blue-600 transition-all">Sign In</a></p>
      </div>
    </div>
  </nav>
</template>
<style scoped>
nav {
  color: #070f18;
}
nav ul li a {
  display: block;
}
.active {
  font-weight: bolder;
}
.showModal {
  display: block;
}
.showMenu {
  max-height: 400px;
  padding-top: 1.9rem;
  padding-bottom: 1.9rem;
}
</style>
