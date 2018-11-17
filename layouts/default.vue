<template>
  <div class="contaner">
    <header class="flex-container">
   <div class="social-block">
     <ul>
       <li><a href="#"><i class="fa fa-facebook"></i></a></li>
       <li><a href="#"><i class="fa fa-vk"></i></a></li>
       <li><a href="#"><i class="fa fa-instagram"></i></a></li>
       <li><a href="#"><i class="fa fa-youtube-play"></i></a></li>
     </ul>
   </div>
   <div class="links-block"> 
     <ul>
       <li>
         <nuxt-link to="/">home</nuxt-link>
       </li>
       <li>
         <nuxt-link to="/gallery">gallery</nuxt-link>
       </li>
       <li>
         <nuxt-link to="/about">about</nuxt-link>
       </li>
       <li>
         <nuxt-link to="/contact">contact</nuxt-link>
       </li>
       <li>
         <nuxt-link to="/temp">temp</nuxt-link>
       </li>
     </ul>
   </div>
    </header>
    <nuxt/>
    <footer>
      <p>©by Diana {{ year}}</p>
    </footer>
  </div>
</template>

<style>
body {
  margin: 0;
}

footer p{
  text-align: center;
}
h1, h2 {
  font-family: 'Dancing Script', cursive;
}
  a{
    color:black
  }
  .contaner {
  max-width: 1000px;
  margin: 0 auto;
  }
  .fa-facebook:hover {
    color:#3B5998
  }
.fa-vk:hover{
  color:#4c75a3
}
.fa-instagram:hover {
  color:#a1182f
}
.fa-youtube-play:hover{
  color:#ad1414
}


.flex-container{
  display: flex;
  flex-direction: row;
}

.social-block{
    width: 25%
}

.social-block > ul > li {
  display: inline-block;
  margin-left: 10px;
}

.links-block>ul>li a{
  text-decoration: none;
  text-transform: uppercase;
}

.nuxt-link-exact-active {
  color: #27D3B4
}
.links-block>ul>li{
  display: inline-block;
  margin-left: 15px;
}

.links-block{
  width: 75%;
  text-align: center;
}
body{
  overflow-x: hidden;
}

@media only screen and (max-width: 480px){
  .social-block {
  width: 100%
  }
  .links-block{
    width: 0;
    height: 0;
    visibility: hidden;
  }
}

</style>

<script>
export default {
   data () {
    return {
      year: new Date().getFullYear()
    }
   }
}
</script>