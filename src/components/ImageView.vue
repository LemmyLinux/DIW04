<template>
  <section id="main-img">
      <div class="img-big"> 
          <img v-bind:src="fotos[0]" alt="Silla barcelona blanca">
      </div>
        <div class="img-mini">
          <a @click="cambiarFoto(1)"><img  class="img-ft" v-bind:src="fotos[1]" alt="Silla barcelona blanca" copyright="'A white Barcelona chair' by eston is licensed under CC BY-NC-SA 2.0" ></a>
          <a @click="cambiarFoto(2)"><img  class="img-ft" v-bind:src="fotos[2]" alt="Silla barcelona marron" copyright="'Mies van der Rohe Barcelona Chair' by Andy Field (Field Office) is licensed under CC BY-NC-SA 2.0" ></a>
          <a @click="cambiarFoto(3)"><img  class="img-ft" v-bind:src="fotos[3]" alt="Silla barcelona negro" copyright="'barcelona chair' by jennypdx is licensed under CC BY-ND 2.0" ></a>
          <a @click="cambiarFoto(4)"><img  class="img-ft" v-bind:src="fotos[4]" alt="Silla barcelona bison" copyright="'Barcelona Chair' by hyfen is licensed under CC BY-NC-SA 2.0" ></a>
        </div>
      </section>    
</template>

<script>
export default {
    Name: 'ProductoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/blanco.jpg'),
                require ('../assets/blanco.jpg'),
                require ('../assets/marron.jpg'),
                require ('../assets/negro.jpg'),
                require ('../assets/bison.jpg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }

}
</script>

<style escoped>
.img-ft{
    width: 200px;
    height: 150px;
}

#main-img {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
}

.img-mini {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}

.img-mini img {
    width: 100px;
    border:2px solid #d8d8d8;
    
}
</style>