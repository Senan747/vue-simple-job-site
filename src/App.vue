<template>
  <nav>
    <router-link to="/">Home</router-link> 
    <router-link :to="{ name: 'about' }">About</router-link> 
    <router-link to="/jobs">Jobs</router-link>
  </nav>
  <router-view/>

  
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
}

nav {
  display:flex;
  justify-content: center;
  padding: 30px;
  
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
