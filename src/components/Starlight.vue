<template>
  <hr class="star-light my-5">
</template>

<script>
  export default{
    name: 'starlight'
  }
</script>

<style>
  hr.star-light{
    width: 250px;
    border:none;
    border-top: 5px solid;
  }
  hr.star-light::after{
    font-family: FontAwesome;
    content: '\f005';
    font-size:2rem;
    position:relative;
    top:-.8em;
    background-color: #18BC9C;
    padding:8px;
  }
</style>
