<template>
  <main-nav />
  <hero />
  <cards-container/>
  <img-card/>
  <testimonial-container/>
  <contact/>
  <main-footer />

</template>

<script>
import mainNav from './components/main-nav.vue'
import hero from './components/hero.vue';
import cardsContainer from './components/cards-container.vue';
import imgCard from './components/img-card.vue';
import TestimonialContainer from './components/testimonial-container.vue';
import Contact from './components/contact.vue';
import mainFooter from './components/main-footer.vue';

export default {
  name: 'app',
  data() {
    return {
    }
  },
  components: {
    mainNav,
    hero,
    cardsContainer,
    imgCard,
    TestimonialContainer,
    Contact,
    mainFooter
  }
}

</script>