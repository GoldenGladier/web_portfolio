<template>
  <div id="app">
    <!-- <header class="menu">
        <div class="icon">
            <i class="bi bi-list"></i>
        </div>
        <div class="nav">
            <router-link to="/" class="item-nav">
              <lord-icon
                  src="https://cdn.lordicon.com/gmzxduhd.json"
                  trigger="loop"
                  colors="primary:#ffffff,secondary:#3877dc"
                  style="width:250px;height:250px">
              </lord-icon>            
              Home
            </router-link>
            <router-link to="/aboutme" class="item-nav">Más de mi</router-link>
            <router-link to="/academic" class="item-nav">Formación</router-link>
            <router-link to="/criptography" class="item-nav">Criptografía</router-link>
            <a href="/public_key_Omar.rsa" download class="item-nav">Mi llave pública</a>          
        </div>
    </header> -->
    <!-- <router-view/> -->
    <Home />
    <Navbar />
    <Skills />
    <Projects />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Nav.vue';
import Home from './components/Home.vue';
import Skills from './components/Skills.vue';
import Projects from './components/Projects.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components : {
    Navbar,
    Home,
    Skills,
    Projects,
    Footer,
  },
}
</script>

<style>
/* -------- Fonts ------- */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
/* font-family: 'Open Sans Condensed', sans-serif; */
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Fuggles&display=swap');
/* font-family: 'Fuggles', cursive;  */
@import url('https://fonts.googleapis.com/css2?family=Abel');
/* font-family: 'Abel', sans-serif; */
/* ---------------------- */

/* ----- Global variables ----- */
:root {
  --color-background-blue: #0D4497;
  --color-font-main-light: azure;
  --color-font-secondary-light: #D1D1D1;
}
/* ---------------------------- */

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

</style>
