<template>
  <div class="about">
    <Hero v-bind:title="title" />
    <h1>This is an about page</h1>
  </div>
</template>

<script>
import Hero from '@/components/Hero.vue'
export default {
  name: 'About',
  components: {
    Hero
  },
  data () {
    return {
      title: 'Maurice Project About Page'
    }
  }
}
</script>
