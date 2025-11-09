<script>
import HeaderSection from './components/Header.vue';
import Hero from './components/Hero.vue';
import Services from './components/Services.vue';
import Portfolio from './components/Portfolio.vue';
import ContactForm from './components/Form.vue';
import FooterSection from './components/Footer.vue';

export default {
  components: {
    HeaderSection,
    Hero,
    Services,
    Portfolio,
    ContactForm,
    FooterSection
  }
};
</script>

<template>
  <HeaderSection />
  <Hero />
  <Services />
  <Portfolio />
  <ContactForm />
  <FooterSection />
</template>

<style scoped>

</style>
