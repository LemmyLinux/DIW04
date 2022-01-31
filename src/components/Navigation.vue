<template>
<section id="navigation">
    <div class="container">
    <nav>
        <ul>
            <li><a href="#">HOME</a></li>
            <li><a href="#">MOBILIARIO</a></li>
            <li><a href="#">TEXTIL</a></li>
            <li><a href="#">ESCULTURAS</a></li>
            <li><a href="#">CUADROS</a></li>
            <li><a href="#">RELOJES</a></li>
            <li><a href="#">LÁMPARAS</a></li>
        </ul>
    </nav>
    <div class=grupo>
        <a class="login" href="#">LOGIN</a>
        <a class="registro" href="#">REGISTRO</a>
    </div>
</div>
</section>
  
</template>

<script>
export default {

}
</script>

<style>
section#navigation {
    background: #dd91dd;
    z-index:999;
    padding:0.7rem;
}

section#navigation .container {
    display: flex;
    justify-content: space-between;
}

section#navigation .container nav ul {
    display:flex;
    list-style: none;
    padding: 0;
    margin:0rem 0.7rem;
}
section#navigation .container nav ul li a, .registro:hover, .login:hover{
    background-color: #dd91dd;
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding-left: 1rem;
    padding-right: 1rem;
}
section#navigation .container nav ul li a:hover,.active, .registro, .login {

    background-color:black;
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding: 1rem;
}




</style>