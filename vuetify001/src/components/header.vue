<template>
    <header id="header">
        <div class="container">
            <img src="../../src/assets/logo.png" alt="logo" width="60px">
            <h1> {{ HeaderTitle }} </h1>
            <ul>
                <li v-for='(li, index) in HeaderMenu' v-bind:key="index">
                  <a v-bind:href="li.adresa"> {{ li.menoLinku }} </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
  data () {
    return {
        HeaderTitle: 'Nadpis z hlavného headeru',
        HeaderMenu: [
          {adresa: '#', menoLinku: 'O mne'},
          {adresa: '#', menoLinku: 'Životopis'},
          {adresa: '#', menoLinku: 'Galéria'},
          {adresa: '#', menoLinku: 'Referencie'}
        ]
    }
  }
}
</script>

<style scoped>
#header {
    background: #cecccc;
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

h1 {
    margin-right: 1rem ;
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
  margin: 0.15rem;
  cursor: pointer;
  color: #54b983;
  text-decoration: none;
  font-weight: 800;
  border-bottom: 1px solid #34495e;
}

.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 5% 0 5%;
    border-bottom: 2px solid black;
}
</style>
