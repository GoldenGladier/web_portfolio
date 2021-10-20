<template>
    <a :href="link" class="item-nav" :class="{ active: active }" @click="activate">{{ text }}</a>
</template>

<script>
export default {
  name: 'Presentation',
  props: {
    link: String,
    text: String,
    active: Boolean,
  },
  methods: {
    activate : function (){
      this.$emit('changeSelect');
      this.active = true;      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
