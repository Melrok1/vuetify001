<template>
  <html>
    <app-header></app-header>
    <main-content></main-content>
  </html>
</template>

<script>
import Header from './components/header.vue';
import MainContent from './components/mainContent.vue';

export default {
  components: {
    'app-header': Header,
    'main-content': MainContent
  },
  data () {
    return {
    }
  }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
