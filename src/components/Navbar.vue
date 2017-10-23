<template>
  <b-navbar toggleable="md" type="dark" variant="info" :sticky="true" v-b-scrollspy>

    <b-navbar-brand href="#">Abdallah Ramadan Awwad</b-navbar-brand>

    <b-nav-toggle target="nav_collapse" >
      MENU
      <span class="navbar-toggler-icon"></span>
    </b-nav-toggle>

    <b-collapse is-nav id="nav_collapse">

      <!-- Right aligned nav items -->
      <b-nav is-nav-bar class="ml-5">
        <b-nav-item v-for="item in navItems" :href="item.href" :key="item.title">{{ item.title }}</b-nav-item>
      </b-nav>

    </b-collapse>
  </b-navbar>
</template>

<script>
  export default {
    name: 'navbar',
    data () {
      return {
        navItems: [{
          title: 'skills',
          href: '#skills'
        },
        {
          title: 'portoflio',
          href: '#portfolio'
        },
        {
          title: 'about',
          href: '#about'
        },
        {
          title: 'contact',
          href: '#contact'
        }]
      }
    }
  }
</script>

<style scoped>
  .navbar {
    font-family: 'Montserrat', sans-serif;
    font-weight: bold;
    padding:35px 10%;
    text-transform: uppercase;
    transition: padding .4s;

  }
  .navbar--blw{
    padding:0px 10px;
  }
  a.navbar-brand {
    font-size: 2em;
  }
  .navbar--blw a.navbar-brand{
    font-size:1.3em;
  }
  #nav_collapse{
    font-size: 1.3em;
  }
  #nav_collapse a.nav-link:hover{
    color:#18BC9C;
  }
  #nav_collapse a.nav-link.active{
    background-color:#18BC9C;
    /*padding:3px;*/
    border-radius: 8px;
    color:white;
  }
</style>
