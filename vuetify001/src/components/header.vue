<template>
    <header id="header">
        <div class="container">
            <img src="../../src/assets/logo.png" alt="logo" width="60px">
            <h1> {{ HeaderTitle }} </h1>
            <ul>
                <li><a href="#"></a>O mne</li>
                <li><a href="#"></a>Galeria</li>
                <li><a href="#"></a>Referencie</li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
  data () {
    return {
        HeaderTitle: 'Nadpis z hlavného headeru'
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
  color: #42b983;
}

.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 5% 0 5%;
}
</style>
