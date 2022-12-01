<template>
    <main class="main">
      <d-header></d-header>
      <d-home></d-home>
      <d-about></d-about>
      <d-skills></d-skills>
      <d-qualification></d-qualification>
      <!-- <section class="services section" id="services"></section> -->
      <d-portfolio></d-portfolio>
      <!-- <section class="testimonial section"></section> -->
      <d-contact></d-contact>
    </main>
    <d-footer></d-footer>
</template>

<script>
import dHome from './components/dHome.vue'
import dAbout from './components/dAbout.vue'
import dSkills from './components/dSkills.vue'
import dQualification from './components/dQualification.vue'
import dPortfolio from './components/dPortfolio.vue'
import dContact from './components/dContact.vue'
import dHeader from './components/dHeader.vue'
import dFooter from './components/dFooter.vue'

export default {
  name: 'App',
  components: {
    dHome,
    dAbout,
    dSkills,
    dQualification,
    dPortfolio,
    dContact,
    dHeader,
    dFooter
  }
}
</script>

<style src = "./assets/style/style.css" lang = "css">

</style>
