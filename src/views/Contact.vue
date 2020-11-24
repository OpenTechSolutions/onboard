<template>
  <div>
    <Hero v-bind:title="title" id="bgImg" />
    <ContactForm />
  </div>
</template>

<script>
import Hero from '@/components/Hero.vue'
import ContactForm from '@/components/ContactForm'

export default {
  name: 'Contact',
  components: {
    Hero,
    ContactForm
  },
  data () {
    return {
      title: 'Maurice Project Contact Page'
    }
  }
}
</script>

<style scoped>
  #bgImg{
    background-image: url('../assets/img/2.jpg');
    background-size: cover;
  }
</style>
