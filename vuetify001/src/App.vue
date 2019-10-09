<template>
  <html>
    <app-header></app-header>
    <main-content></main-content>
    <prog-menu v-bind:progMenu="progMenu"></prog-menu>
  </html>
</template>

<script>
import Header from './components/header.vue';
import MainContent from './components/mainContent.vue';
import ProgMenuButton from './components/progMenu.vue';

export default {
  components: {
    'app-header': Header,
    'main-content': MainContent,
    'prog-menu': ProgMenuButton
  },
  data () {
    return {
      progMenu: [
        {adresa: 'https://www.pngfly.com/png-r1hbmm/download.html', menoPolozky: 'HTML', ikona: ''},
        {adresa: 'https://mycolor.space/gradient?ori=to+top&hex=%23051937&hex2=%23A8EB12&sub=1', menoPolozky: 'CSS', ikona: ''},
        {adresa: '#', menoPolozky: 'JavaScript', ikona: ''},
        {adresa: '#', menoPolozky: 'Vue.js', ikona: ''},
        {adresa: '#', menoPolozky: 'Node.js', ikona: ''}
      ]
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
