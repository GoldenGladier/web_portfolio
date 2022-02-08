<template>
  <header :class="'navbar ' + open_menu">
    <button class="icon" @click="handdle_menu">
        <i class="bi bi-list"></i>
    </button>

    <transition name="stretch">
      <div class="nav" v-show="open_menu == true" >
          <a class="item-nav" @click="scrollToElement('banner')">Presentación</a> 
          <a class="item-nav"  @click="scrollToElement('skills')">SKILLS</a>                 
          <a class="item-nav"  @click="scrollToElement('selected-projects')">PROYECTOS</a>
      </div>
    </transition>

  </header>
</template>

<script>
export default {
  name: 'Navbar',
  data(){
      return {
        open_menu : false,
      }
  },
  methods : {
    handdle_menu : function(){
      this.open_menu = !this.open_menu;
    },
    scrollToElement : function(id){
      const element = document.getElementById(id);
      if(element){
        element.scrollIntoView({
          behavior: "smooth"
        });   
      }
      else{
        console.log("Sorry, the section and/or reference (" + id + ") you are trying to scroll to does not exist.")
      }
   
    }, 

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

header.navbar{
    position: fixed;
    top: 10px;
    right: 10px;
    z-index: 100;

    width: auto;
    height: auto;

    transition: 0.3s;
    background: transparent;
    overflow: hidden;
}
header.navbar.true{
    height: calc(100vh - 10px - 10px);
    bottom: 10px;
}


.icon{
    position: relative;
    z-index: 110;

    font-size: 22pt;
    padding: 5px 10px;    

    color: azure;
    background: #313B4D;
    border: none;
    cursor: pointer;
}

.nav{
    padding: 15px 0 0px 9px; 
    height: 100%;

    background: #313B4D;
    color: azure;
    overflow: hidden;
    z-index: 1;
}
.item-nav{
    display: block;
    writing-mode: vertical-rl;
    padding: 0.6rem;
    text-transform: uppercase;
    text-decoration: none;
    color: azure;
    position: relative;

    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 13pt;

    cursor: pointer;
}
.item-nav:hover{
    background: #364959;
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
    top: calc(50% - 2px);
    margin-right: 5rem;
}

/* Animation menu */
.stretch-enter-active {
  animation: stretch-in .5s;
}
.stretch-leave-active {
  animation: stretch-out .5s;
}

@keyframes stretch-in {
  0% {
    transform: translateY(-100%);
  }
  20%{
    transform: translateY(-45%);
  }
  100% {
    transform: translateY(0);
  }
}

@keyframes stretch-out {
  0% {
    transform: translateY(0);    
  }
  20%{
    transform: translateY(-35%);
  }
  100% {
    transform: translateY(-100%);
  }
}
</style>
