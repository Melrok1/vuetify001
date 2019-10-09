<template>
    <div id="skill">
        <ul>
            <li v-for="(link, index) in progMenu" v-bind:key="index">  
                <a v-bind:href="link.adresa"> {{ link.menoPolozky }} </a>
            </li>
        </ul>
    </div>
</template>




<script>
export default {
  props: ['progMenu'],
  data () {
    return {}
  }
}
</script>





<style scoped>
#skill {
    background: #cecccc;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    width: 15%;
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
  display: block;
  margin: 0 10px;
  margin-top: 0.4rem;
}

a {
  margin: 0.15rem;
  cursor: pointer;
  color: #54b983;
  text-decoration: none;
  font-weight: 800;
}
</style>
