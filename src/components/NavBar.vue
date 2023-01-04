<template>
<div id="header">
<div class="container">
<nav>
<img src="../assets/fs.svg" class="logo"/>
<ul>
<li><a href="#">Home</a></li>
<li><a href="#">About</a></li>
<li><a href="#">Services</a></li>
<li><a href="#">Contact</a></li>
</ul>
 </nav>
             <div class="header-text">
             <!-- <p>Hello <span>World</span></p> -->
             <h1 class="shine">FUTURE SHOCK</h1>
            </div>  
         
<div class="social-hero">      
<img src="../assets/discord.svg">
<img src="../assets/github.svg">
<img src="../assets/instagram.svg">
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
    background-size:cover;
    background-position:center;
 }
 .social-hero{
   text-align: center;
   margin-top: 5%;
   padding-left: 20px;
   justify-content: space-between;
}
 .container{
padding: 10px 10%;
 }
nav{
    display: flex;
    align-items: center;
    justify-content:space-between;
    flex-wrap: wrap;
    padding-right: 45%;
 }
 .logo{
    width: 100px;
    display: flex;
    align-items: center;
    justify-content:space-between;
    flex-wrap: wrap;
    margin-left: 20%;
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
    margin-top: 5%;
    font-size: 20px;
 }
.header-text h1{
    font-size: 205px;
    width: 1513px;
    font-weight: 800;
    font-family: HudsonNYPro,sans-serif;
    text-align: center;
    line-height: 80%;
}
.header-text p span{
    color: #ff004f;
}
#shape{
   width: 500px;
   margin-left: 900px;
   margin-top: -20%;
}

/*shine h1 */
h1.shine:hover {
  mask-image: linear-gradient(-75deg, rgba(218, 215, 215, 0.6) 30%, #000 50%, rgba(255, 255, 255, 0.6) 70%);
  mask-size: 200%;
  animation: shine 1s infinite;
}

@keyframes shine {
  from {
    -webkit-mask-position: 150%;
  }
  
  to {
    -webkit-mask-position: -50%;
  }
}

</style>
