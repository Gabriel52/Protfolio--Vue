<template>
  <div id="app">
    <Header />
    <ShowCase msg="Welcome to Your Vue.js App"/>
    <AboutSection />
    <ServicesSection/>
    <PortfolioSection />
    <ContactSection />
    <Footer />
  </div>
</template>

<script>
import ShowCase from './components/ShowCase.vue'
import Header from './components/Header.vue'
import AboutSection from './components/AboutSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import PortfolioSection from './components/PortfolioSection.vue'
import ContactSection from './components/ContactSection.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    ShowCase,
    Header,
    AboutSection,
    ServicesSection,
    PortfolioSection,
    ContactSection,
    Footer,
  }
}
</script>

<style>
  #app {
    margin: 0;
    padding: 0;
    outline:0;
    box-sizing: border-box;

  }
  body {
    font-family: 'Open Sans', sans-serif;
    background: #f0f0f5;
    -webkit-font-smoothing:antialiased;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  html{
    scroll-behavior: smooth;
  }
</style>
