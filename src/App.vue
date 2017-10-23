<template>
  <div>
    <navbar></navbar>
    <intro></intro>
    <skills></skills>
  </div>
</template>

<script>
  import Navbar from './components/Navbar.vue'
  import Intro from './components/Intro.vue'
  import Skills from './components/Skills.vue'
  export default {
    name: 'app',
    components: {
      Navbar,
      Intro,
      Skills
    }
  }
</script>

<style lang="scss">
  @import "style/main";

</style>
