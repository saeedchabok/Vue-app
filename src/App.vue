<template>
    <HeaderApp title="Vue.js" :titleD="title" :extD="ext"/>
</template>

<script>
import HeaderApp from './components/Header.vue'

export default {
  name: 'App',
  data: () => ( {
    title: 'Vue',
    ext: true
  }),
  components: {
    HeaderApp
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
