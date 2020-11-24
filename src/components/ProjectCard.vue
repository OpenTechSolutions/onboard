<template>
  <div class="flex flex-wrap justify-center">
    <div v-for="project in projects" v-bind:key="project.id">
      <div class="w-64 bg-white m-3 shadow">
        <img :src=project.url alt="">
        <h4 class="px-4 py-4 font-bold text uppercase" id="truncate">{{project.title}}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectCard',
  props: ['projects']
}
</script>

<style>
  #truncate {
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  }
</style>
