<template>
  <header class="menu">
      <div class="icon">
          <i class="bi bi-list"></i>
      </div>
      <div class="nav">
          <a href="#" class="item-nav active">Home</a>
          <a href="#" class="item-nav">About me</a>
          <!-- <a href="#" class="item-nav active">Portfolio</a>
          <a href="#" class="item-nav">Contact</a> -->
          <ItemNav link="#" text="Portfolio" :active="activate_all" v-on:changeSelect="deactivateAll"/>
          <ItemNav link="#" text="Contact" :active="activate_all" v-on:changeSelect="deactivateAll"/>
          <ItemNav link="#" text="Other" :active="activate_all" v-on:changeSelect="deactivateAll"/>
      </div>
  </header>
</template>

<script>
import ItemNav from './ItemNav.vue';

export default {
  name: 'Presentation',
  components: {
      ItemNav,
  },
  data: function () {
    return {
      activate_all: false,
    }
  },
  methods: {
      deactivateAll: function(){
        this.activate_all = false;
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.menu{
    background: #313B4D;
    color: azure;
    position: absolute;
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
.active{
    background: #3d4961;
}
.active::after{
    content: "";
    display: block;
    height: 2px;
    width: 100%;
    z-index: 6;
    border-radius: 50%;
    background: azure;
    position: absolute;
    top: 49%;
    margin-right: 10px;
}
</style>
