<template>
  <section id="searchbar">
      <form @submit.prevent="handleSubmit">
          <input type="text" placeholder="Click para buscar">
          <button class="boton">Buscar</button>
      </form>
  </section>
</template>

<script>
export default {
    name: 'SearchBar',
    methods: {
        handleSubmit() {
            console.log("Busqueda enviada")
        }
    }
}
</script>

<style>
section#searchbar {
    margin: 1rem;
}
section#searchbar form {
    display: flex;
    justify-content: left;
    align-items: center;
}
section#searchbar input{
    margin: 1rem;
    padding: 0.7rem 1rem;
    border-style: solid;
    border: 2px solid #dd91dd;
    color: #181818;
    outline: none;
    line-height: 1.4rem;
    border-radius: 25px;
    font-size: 1.2rem;
}


</style>