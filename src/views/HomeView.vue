<script setup>
import Nav from '../components/Nav.vue'
import Header from '../components/Header.vue'
import Features from '../components/Features.vue'
import Services from '../components/Services.vue'
import Testimonial from '../components/Testimonial.vue'
import CTA from '../components/CTA.vue'
import Footer from '../components/Footer.vue'
</script>
<template>
  <div class="py-12 px-12 font-Poppins md:px-20">
    <Nav />
    <Header />
    <Features />
    <Services />
    <Testimonial />
  </div>
  <CTA />
  <Footer />
</template>
