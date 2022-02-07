<template>

    <div class="skill" :style="cssProps">
        <div class="skill-information">
            <p class="skill-name">{{ skill_name }}</p>
            <p class="skill-level">{{ skill_level }}%</p>
        </div>
        <div class="skill-bar"></div>
    </div>

</template>

<script>
export default {
  name: 'SkillBar',
  props : {
      skill_name : String,
      skill_level : String,
  },
  computed: {
    cssProps() {
      return {
        '--skill-level': this.skill_level + "%",
      }
    }
  }  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
    font-family: 'Open Sans Condensed', sans-serif;
    font-size: 15pt;
}
.skill-information{
    position: relative;
    display: block;
}
.skill-information .skill-name{
    display: inline-block;
    float: left;
}
.skill-information .skill-level{
    display: inline-block; 
    float: right;
}

.skill-bar{
  position: relative;
  background: #f1f1f1;
  width: 100%;
  height: 0.5rem;
  border-radius: 1rem;
  margin: auto;
  overflow: hidden;
}
.skill-bar::after{
  content: '';
  position: absolute;
  left: 0;
  /* background: #0D4497; */
  background: #3877DC;
  width: var(--skill-level, 0%);
  height: 0.5rem;
  border-radius: 1rem;
}
</style>

