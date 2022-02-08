<template>
    <div class="project">
        <div class="project-info">
            <a :href="project_url" target="_blank" class="projectLink">
                <img :src="'./' + project_img" :alt="project_img" class="project-banner">
                <h6 class="project-name">{{ project_name }}</h6>
            </a> 
            
            <!-- <div class="info-fixed">
                <h6 class="project-name">Escom Groups</h6> 
                <a href="#" class="button btn-view-project">Visitar proyecto</a>
            </div> -->
                
            <transition name="stretch" mode="out-in" appear>  

                <div class="info-dropdown" v-if="info_dropdown == true" key="dropdown-active">
                    <button class="btn-none" @click="handleDropdown">
                        <i class="bi bi-chevron-up"></i>
                        Cerrar
                    </button>
                    <p class="project-description">
                        {{ project_description }}
                    </p>
                </div>

                <div class="info-dropdown dropdown-inactive" v-else key="dropdown-inactive">
                    <button class="btn-none" @click="handleDropdown">
                        Detalles
                        <i class="bi bi-chevron-down"></i>
                    </button>
                </div> 

            </transition>   

        </div>
    </div>
</template>

<script>
export default {
  name: 'Project',
  props : {
      project_name : String,
      project_description : String,
      project_url : String,
      project_img : String,
  },
  data() {
    return{
        info_dropdown : false,
    }
  },
  methods : {
      handleDropdown : function(){
        this.info_dropdown = !this.info_dropdown;
      }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.project{
  background: #ffffff;
  border: solid 1px #e9e9e9;
  border-radius: 7px;
  overflow: hidden;
  align-self: flex-start;
}

.projectLink{
    text-decoration: none;
}

img.project-banner{
    width: 100%;
    position: relative;
    z-index: 5;
}

.info-fixed{
    display: inline-block;
    width: 100%;
    padding: 20px;
    padding-bottom: 0;
    margin: 0;
    box-sizing: border-box;
}

.project-name{
  font-family: 'Open Sans Condensed', sans-serif;
  font-weight: lighter;
  text-decoration: none;
  color: #313B4D;
  font-size: 20pt;
  z-index: 100;
}

.info-fixed .project-name{
  float: left;
}

.btn-view-project{
    display: inline-block;
    text-decoration: none;
    padding: 8px;
    border-radius: 5px;
    background: #0D4497;
    color: azure;
    transition: 0.4s;
    float: right;
}
.btn-view-project:hover{
    background: #3877DC;
    transition: 0.4s;
}

.info-dropdown .project-description{
    padding: 20px;
    padding-top: 0;

    font-family: 'Abel', sans-serif;
    font-size: 13pt;
    text-align: justify;
}

.btn-none{
    padding: 5px 15px;
    padding-bottom: 0;
    margin: 0;
    cursor: pointer;
    font-size: 15pt;
    background: transparent;
    border: none;

    display: inline-grid;

    color: var(--color-font-secondary-light);
    font-size: 12pt;    
    font-family: 'Open Sans Condensed', sans-serif;
}

.dropdown-inactive .btn-none{
    padding: 5px 15px;
    padding-bottom: 0;
}

.btn-none i{
  animation: pulse 1.5s infinite linear;
}

/* Animation Project */
.stretch-enter-active {
  animation: stretch-in .5s;
}
.stretch-leave-active {
  animation: stretch-in reverse .5s;
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

.diffuse-enter-active {
  animation: diffuse 1s ease-in reverse;
}

@keyframes pulse{
    0%{
        transform: scale(1);
    }
    25%{
        transform: scale(0.8);
    }
    50%{
        transform: scale(1);
    }
    75%{
        transform: scale(1.3);
    }
    100%{
        transform: scale(1);
    }
}

</style>

