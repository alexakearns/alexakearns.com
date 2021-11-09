<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/projects">Projects</router-link> |
    <router-link to="/contact">Contact</router-link>
  </div>
  <router-view />
</template>

<style>
body {
  background-color: #000;
  margin: 0px;
  overflow: hidden;
  padding: 0px;
}

#app {
  background-image: url(assets/portfolio-background_2.jpg);
  background-position: center;
  background-size: cover;
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  position: relative;
  text-align: center;
  width: 100vw;
}

#nav {
  padding: 30px;
  display: table;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a:hover {
  font-weight: bold;
  color: pink;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
