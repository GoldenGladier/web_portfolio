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
                
            <div class="info-dropdown" v-if="info_dropdown">
                <button class="btn-none" @click="handleDropdown"><i class="bi bi-chevron-up"></i></button>
                <p class="project-description">
                    {{ project_description }}
                </p>
            </div>

            <div class="info-dropdown dropdown-inactive" v-else>
                <button class="btn-none" @click="handleDropdown"><i class="bi bi-chevron-down"></i></button>
            </div>            
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
  font-weight: bold;
  text-decoration: none;
  color: #313B4D;
  font-size: 20pt;
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
    /* margin-top: 1rem; */
    text-align: justify;
    padding: 20px;
    padding-top: 0;
}

.btn-none{
    padding: 10px 15px;
    margin: 0;
    cursor: pointer;
    font-size: 15pt;
    background: transparent;
    border: none;
}

.dropdown-inactive .btn-none{
    padding: 5px 15px;
    padding-bottom: 0;
}

@keyframes pulse{
    0%{
        transform: scale(1);
    }
    50%{
        transform: scale(2);
    }
    100%{
        transform: scale(1);
    }
}

.btn-none i{
  animation-duration: 1s;
  animation-name: pulse !important;
  animation-iteration-count: infinite;
}


</style>

