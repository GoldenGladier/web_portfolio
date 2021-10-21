<template>
  <div id="app">
    <header class="menu">
        <div class="icon">
            <i class="bi bi-list"></i>
        </div>
        <div class="nav">
            <router-link to="/" class="item-nav">Home</router-link>
            <router-link to="/aboutme" class="item-nav">Más de mi</router-link>
            <router-link to="/academic" class="item-nav">Formación</router-link>
            <router-link to="/criptography" class="item-nav">Criptografía</router-link>
            <router-link to="/#" class="item-nav">Mi llave pública</router-link>          
            <!-- <a href="#" class="item-nav active">Portfolio</a>
            <a href="#" class="item-nav">Contact</a> -->
        </div>
    </header>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body, *{
  margin: 0;
  padding: 0;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

.menu{
    background: #313B4D;
    color: azure;
    position: fixed;
    height: 100vh;
    z-index: 5;
    right: 0;
    display: flex;
    justify-content: center;
    align-items: center;
}
.icon{
    font-size: 22pt;
    position: absolute;
    top: 15px;
}
.nav{
    padding-left: 20px;
    overflow: hidden;
}
.item-nav{
    display: block;
    writing-mode: vertical-rl;
    padding: 15px 20px 15px 5px;
    text-transform: uppercase;
    text-decoration: none;
    color: azure;
    position: relative;
}
a.router-link-exact-active, .active{
    background: #3d4961;
}
a.router-link-exact-active::after, .active::after{
    content: "";
    display: block;
    height: 2px;
    width: 100%;
    z-index: 6;
    border-radius: 20%;
    background: azure;
    position: absolute;
    top: 49%;
    margin-right: 10px;
}
</style>
