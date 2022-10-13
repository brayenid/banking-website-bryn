<script setup>
import Clock from '../icons/Clock.vue'
import Support from '../icons/Support.vue'
import Mail from '../icons/Mail.vue'
import Phone from '../icons/Phone.vue'
</script>
<template>
  <footer>
    <div class="infos">
      <div class="info sm:max-w-xs">
        <h3>Company Info</h3>
        <p class="mt-3">Reach out to us anytime and lets create a better future for all technology users together, forever. We are open to all types of collab offers and tons more.</p>
        <div class="subInfo">
          <Clock />
          <span>
            Office Hours <br />
            Monday-Friday 9 AM-5 PM PST
          </span>
        </div>
        <div class="subInfo">
          <Support />
          <span>
            Support Hours <br />
            24/7 365
          </span>
        </div>
      </div>
      <div class="info">
        <h3>Contact Info</h3>
        <div class="subInfo">
          <Mail />
          <span>info@gmail.com</span>
        </div>
        <div class="subInfo">
          <Phone />
          <span>858-227-4878</span>
        </div>
      </div>
      <div class="info">
        <h3>Our Services</h3>
        <ul class="mt-3">
          <li>Information Systems Strategy</li>
          <li>Custom Software</li>
          <li>Integration Services</li>
          <li>Business Automation</li>
          <li>Web, Ecommerce & Mobiel Apps</li>
          <li>Creative</li>
        </ul>
      </div>
      <div class="info">
        <h3>Our Location</h3>
        <img class="mt-3" src="../../img/footer/Techyes map-01 3.png" alt="" />
      </div>
    </div>
    <div class="text-center pt-7">
      <p>© 2022 abci - All rights reserved. - Created by <a href="https://brayenluhat.xyz" target="_blank">Brayen Luhat</a> - UI by uidesign.to</p>
    </div>
  </footer>
</template>
