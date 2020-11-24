<template>
  <div class="about">
    <Hero v-bind:title="title" />
    <div class="container m-auto my-10">
    <project-card v-bind:projects="projects"/>
    </div>
  </div>
</template>

<script>
import Hero from '@/components/Hero.vue'

import axios from 'axios'
import ProjectCard from '../components/ProjectCard.vue'
export default {
  name: 'About',
  components: {
    Hero,
    ProjectCard
  },
  data () {
    return {
      title: 'Maurice Project About Page',
      projects: []
    }
  },
  created () {
    axios.get('https://jsonplaceholder.typicode.com/photos?_limit=4')
      .then(response => (this.projects = response.data))
  }
}
</script>
