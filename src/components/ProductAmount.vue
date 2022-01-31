<template>
  <section id="product">
      <h1>Silla Barcelona</h1>
      <h2>399,99€ <span class="iva">sin IVA: 315,99€</span></h2>
      <div class="wrapper">
          <button class="btn" @click="modifyAmount('-1')" type="button" name="button">-</button>
          <input class="amount" type="text" name="name" :value="productAmount">
          <button class="btn" @click="modifyAmount('1')" type="button" name="button">+</button>
      </div>
      <br>
      <button class="boton"><span class="material-icons">shopping_cart</span> AÑADIR CARRITO</button>
  </section>
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            productAmount: 1
        }
    },
    methods: {
        modifyAmount(num) {
            this.productAmount += +num;
            if (!isNaN(this.productAmount) && (this.productAmount < 0)) {
              this.productAmount = 0
            } 
        }
    }


}
</script>

<style scoped>
section#product {
  flex: 1 1 18rem;
}
h1 {
  font-size: 2.2rem;
}
h2 {
  font-size:1.7rem;
  color: #dd91dd;
}
span.iva {
  font-size:1rem;
  font-weight: normal;
  color: #282828
}
.wrapper {
  height: 2rem;
  display: flex;
}

.amount {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
button:focus, input:focus {
  outline: 0;
}

</style>