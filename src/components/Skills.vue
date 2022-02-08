<template>
    <section class="skills" id="skills">
      <h2>Skills</h2>
      <div class="skills-list">
        <SkillBar skill_name="HTML 5" skill_level="80"/>            
        <SkillBar skill_name="CSS 3" skill_level="50"/>            
        <SkillBar skill_name="Java Script" skill_level="60"/>            
        <SkillBar skill_name="PHP" skill_level="10"/>            
        <SkillBar skill_name="Java" skill_level="60"/>      

        <SkillBar skill_name="Python" skill_level="35"/>            
        <SkillBar skill_name="Django" skill_level="50"/>            
        <SkillBar skill_name="Vue JS" skill_level="55"/>            
        <SkillBar skill_name="React JS" skill_level="25"/>            
        <SkillBar skill_name="Linux" skill_level="60"/> 
        <SkillBar skill_name="SQL" skill_level="50"/> 
        <SkillBar skill_name="Firebase" skill_level="40"/> 
      </div>                  
    </section>
</template>

<script>
import SkillBar from './SkillBar.vue'

export default {
  name: 'Skills',
  components : {
    SkillBar,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.skills h2{
  font-family: 'Open Sans Condensed', sans-serif;
  font-weight: bold;
  font-size: 30pt;
}
.skills-list{
  width: 80%;
  margin: 2rem auto;
  display: grid;
  gap: 2rem;
  grid-template-columns: repeat(auto-fill, minmax(min(100%, 20rem), 1fr)); 
}
</style>

