<template>
  <div>
    <TopBar />
    <HeroVue/>
    <informationVue id="about"/>
    <FeatureVue />
    <planVue id="pricing"/>
    <testimonialVue/>
    <faq/>
    <footerhome/>
  </div>
</template>

<script setup>
import FeatureVue from './components/Feature.vue';
import HeroVue from './components/Hero.vue';
import informationVue from './components/information.vue';
import planVue from './components/plan.vue';
import testimonialVue from './components/testimonial.vue';
import TopBar from './components/TopBar.vue';
import faq from './components/faq.vue';
import footerhome from './components/footer.vue';


</script>

<style>
</style>
