<template>
  <!-- <Loader /> -->
  <SiteNav />
  <Header />
  <Protien />
  <About />
  <Growyhing />
  <Testimonial />
  <Contact />
  <Footer />
</template>

<script>
import Contact from '../components/Contact.vue';
import Footer from '../components/Footer.vue';
import Loader from '../components/Loader.vue';
import SiteNav from '../components/SiteNav.vue';
import Header from '../components/Header.vue';
import Protien from '../components/Protien.vue';
import About from '../components/About.vue';
import Growyhing from '../components/Growyhing.vue';
import Testimonial from '../components/Testimonial.vue';
export default {
    components: { Contact, Footer, Loader, SiteNav, Header, Protien, About, Growyhing, Testimonial }
}
</script>

<style>

</style>