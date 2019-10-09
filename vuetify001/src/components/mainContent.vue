<template>
    <main>
        <article>
            <img src="../assets/img/M.png" alt="M" width="50px">
            <p>
                <span class="importName">{{ meno }}</span> Lorem ipsum, dolor sit amet consectetur 
                adipisicing elit. Commodi nihil 
                cupiditate eos saepe mollitia dignissimos molestias perspiciatis. Placeat 
                dolorem ad <span class="importName">{{ meno }}</span> tenetur illo vel doloribus 
                at libero quo. Quibusdam, error facere?
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea quos velit assumenda, 
                quibusdam harum tenetur, nihil atque aliquam vero voluptatum inventore perferendis 
                illum doloribus quo voluptatibus earum impedit ipsum cumque.
            </p>
            <img src="../assets/img/L.png" alt="M" width="50px">
            <p>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
                <span class="importName">{{ meno }}</span> Commodi nihil 
                cupiditate eos saepe mollitia dignissimos molestias perspiciatis. Placeat 
                dolorem ad tenetur illo vel doloribus at libero quo. Quibusdam, error facere?
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea quos velit assumenda, 
                quibusdam harum tenetur, nihil atque aliquam vero voluptatum inventore perferendis 
                illum doloribus quo voluptatibus earum <span class="importName">{{ meno }}</span> 
                impedit ipsum cumque.
            </p>
        </article>
    </main>
</template>

<script>

export default {
  data () {
    return {
        meno: 'Martin Blaščák'
    }
  }
}
</script>

<style scoped>
main {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 60px 50px;
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

.importName {
    font-weight: 800;
    font-style: italic;
}
</style>
