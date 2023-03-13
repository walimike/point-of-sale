<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <Article/>
</template>

<script>
import Article from './views/Article.vue'

export default {
  name: 'App',
  components: {
    Article
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
