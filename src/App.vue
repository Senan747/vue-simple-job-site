<template>
  <nav>
    <div class="navigation"> <router-link to="/">Ana səhifə</router-link> 
    <router-link :to="{ name: 'about' }">Haqqımızda</router-link> </div>
   
  </nav>
  <router-view/>

  
</template>


<style>
body{
  background-color: #BDDEA5;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}


nav {
  display:flex;
  position: fixed;
  top: 0;
  justify-content: center;
  padding: 30px;
  background-color: #087829;
  width: 100%;
  margin: 0;
}
.navigation{
  margin: 0;
 
}

nav a {
  margin: 10px;
  font-weight: bold;
  color: #2c3e50;
  background-color: #eaf5f0;
  border: none;
  padding:15px 20px;
  border-radius: 10px;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #eaf5f0;
  background-color: red;
  border-radius: 10px;
}
button {
  margin: 0 10px;
  padding: 10px;
  border: none;
  border-radius: 4px;
}
</style>
