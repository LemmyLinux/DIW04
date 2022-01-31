<template>
  <section id="breadcrumb">
      <a class="inicio" href="#"> Home </a> >
      <a href="#">Mobiliario</a> > 
      <a href="#">Mobiliario de diseño</a> > 
      <a href="#">Sillas y sillones </a> > 
      <a class="actual" href="#">Silla Barcelona</a> 


  </section>
</template>

<script>
export default {

}
</script>

<style>
section#breadcrumb {
    margin-left: 1rem;
    display:flex;

}
section#breadcrumb a, 
section#breadcrumb a:hover, 
section#breadcrumb a:visited{
    text-decoration: none;
    font-size: 1.2rem;
    margin-left: 1rem;
    margin-right: 1rem;
    color: #dd91dd;
}
section#breadcrumb a.actual {
    font-weight: 700;
}
section#breadcrumb {
    margin-left: 1rem;
    color: #dd91dd;
}
</style>