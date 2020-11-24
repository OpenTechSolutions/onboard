<template>
  <div class="home">
    <Hero v-bind:title="title" />
    <div class="container m-auto p-5 bg-gray-700">
      <input type="text" placeholder="Enter Search... " class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" />
    </div>
    <div v-for="comment in comments" v-bind:key="comment.id">
      {{comment.name}}
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue'
import axios from 'axios'

export default {
  name: 'Home',
  components: {
    Hero
  },
  data () {
    return {
      title: 'Maurice Project Landing Page',
      comments: []
    }
  },
  created () {
    axios.get('https://jsonplaceholder.typicode.com/comments')
      .then(response => (this.comments = response.data))
  }
}
</script>
