<template>
  <section class="presentation">
    <header class="menu">
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
            <!-- <a href="#" class="item-nav active">Portfolio</a>
            <a href="#" class="item-nav">Contact</a> -->
        </div>
    </header>
  </section>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
