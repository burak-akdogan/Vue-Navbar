<template>
<div id="header">
<div class="container">
<nav>
<img src="../assets/mylogo.png" class="logo"/>
<ul>
<li><a href="#">Home</a></li>
<li><a href="#">About</a></li>
<li><a href="#">Services</a></li>
<li><a href="#">Contact</a></li>
</ul>
 </nav>
             <div class="header-text">
             <p>Hello <span>World</span></p>
             <h1>Lorem  dolor <br> consectetur adipisicing elit. </h1>
            </div>   
</div> 
</div>
</template>
<script >
export default {
    name:'NavBar'

}


</script>
<style lang="scss">
@import './vars.scss';

#header{
    width: 100%;
    height: 100vh;
    /* background-image: url(../assets/header.png); */
    background-size:cover;
    background-position:center;
 }
 .container{
padding: 10px 10%;
 }
 nav{
    display: flex;
    align-items: center;
    justify-content:space-between;
    flex-wrap: wrap;
    padding-right: 15%;
 }
 .logo{
    width: 100px;
 }
 nav ul li{
    display: inline-block;
    list-style: none;
    margin: 50px 30px  ;

 }
 nav ul li a{
    color: $white;
    text-decoration: none;
    font-size: 18px;
    position: relative;

 }
 nav ul li a::after{
    content: '';
    width: 0%;
    height: 3px;
    background: $primary;
    position: absolute;
    left: 0;
    bottom: -7px;
    transition: 0.8s;
 }
 nav ul li a:hover::after{
    width: 100%;
 }
 .header-text{
    margin-top: 10%;
    font-size: 20px;
 }
.header-text h1{
    font-size: 40px;
    margin-top: 20px;
}
.header-text p span{
    color: #ff004f;
}
#shape{
   width: 500px;
   margin-left: 900px;
   margin-top: -20%;
}

</style>