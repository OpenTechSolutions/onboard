<template>
    <div>
        <Hero v-bind:title="title" />
        This is a Contact page
    </div>
</template>

<script>
import Hero from '@/components/Hero.vue'
export default {
  name: 'Contact',
  components: {
    Hero
  },
  data () {
    return {
      title: 'Maurice Project Contact Page'
    }
  }
}
</script>
