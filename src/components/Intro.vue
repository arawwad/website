<template>
  <b-container fluid class="text-center">
    <b-row align-h="center" class="my-5">
      <b-col cols="3">
        <image-placeholder :width="200" :height="200" class="rounded-circle"></image-placeholder>
      </b-col>
    </b-row>
    <b-row align-h="center" class="my-5">
      <b-col cols="7" class="title">
        <h2>Abdallah Ramadan Awwad</h2>
        <starlight></starlight>
        <h2>Web Developer</h2>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
  import ImagePlaceholder from 'vuejs-image-placeholder'
  import Starlight from './Starlight.vue'
  export default {
    components: {
      ImagePlaceholder,
      Starlight
    }
  }
</script>

<style lang="scss" scoped>
  .container-fluid{
    background-color: #18BC9C;
    padding: 120px;
  }

  .title{
    font-weight:bold;
    font-family: 'Montserrat', sans-serif;
    color: #fff;
  }
  .title h2{
    font-size: 4rem;
  }
</style>
