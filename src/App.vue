<template>
  <div class="w-100">
    <div>
      <NavBar />
    </div>
   <!--  py-5 -->
    <div class="">
      <HeroSection/>
      <AboutUs />
      <GoalDiv />
      <ChallangeDiv/>
      <ContactUs/>
    </div>
    <div>
      <FooTeer />
    </div>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import AboutUs from './components/AboutUs.vue'
import GoalDiv from './components/GoalDiv.vue'
import ChallangeDiv from './components/ChallangeDiv.vue'
import ContactUs from './components/ContactUs.vue'

import FooTeer from './components/FooTeer.vue'


export default {
  name: 'App',
  components: {
    NavBar,
    AboutUs,
    GoalDiv,
    HeroSection,
    ChallangeDiv,
    ContactUs,





    FooTeer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}

</style>
