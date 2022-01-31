<template>
<Header />
<Navigation />
<div class="container">
  <SearchBar />
  <BreadCrumb />
  <div class="dos-columnas">
    <ImageView />
    <ProductAmount />
  </div>
  <div class="container">
    <Description />
  </div>
  <div class="container">
    <Video />
  </div>
</div>
  <Footer />

</template>

<script>
import Header from './components/Header.vue'
import Navigation from './components/Navigation.vue'
import SearchBar from './components/SearchBar.vue'
import BreadCrumb from './components/BreadCrumb.vue'
import ImageView from './components/ImageView.vue'
import ProductAmount  from './components/ProductAmount.vue'
import Description from './components/Description.vue'
import Video from './components/Video.vue' 
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: { 
                Header, 
                Navigation, 
                SearchBar, 
                BreadCrumb, 
                ImageView, 
                ProductAmount,
                Description, 
                Video, 
                Footer 
              }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@500&family=Titillium+Web:wght@300;400;700&display=swap');

body{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

#app {
  font-family: 'Titillium Web', rockwell;
}
.container {
    max-width: 1400px;
    margin: auto;
}

.boton {
  background-color: #dd91dd;
  font-size: 1.2rem;
  font-weight: 700;
  color: white;
  padding: 0.7rem 1.2rem;
  cursor: pointer;
  border: none;
}
.dos-columnas {
  display: flex;
  margin: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
