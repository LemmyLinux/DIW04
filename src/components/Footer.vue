<template>
  <footer id="footer">
    <p>© Copyright 2022 - Todos los derechos reservados</p>
    <span id="material-design"><a href="https://material.io/" ><img  src="https://material.io/static/angular/material_logo.1d5336632349ee8653bf.svg" alt="material design logo" copyright="material design by google" /></a></span>
  </footer>
</template>

<script>
export default {

}
</script>

<style>
#footer {
    background-color: #dd91dd;
    display: flex;
    justify-content: flex-start;   /* adjustment */
    position: relative; 
}
#footer p {
    color: white;
    flex: 0 1 auto;
    width: 400px;
    height: 100px; 
    position: absolute;             /* new */
    left: 50%;
    transform: translateX(-50%);
}
#material-design{
  flex: 0 1 auto;
  width: 65px;
  height: 65px;
  margin-left: 12%; 
}
</style>