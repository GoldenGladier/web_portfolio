<template>
  <div class="home">
    <Presentation />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Presentation from '@/components/Presentation.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld,
    Presentation,
  }
}
</script>
