<template>
    <div class="home">
      <NavBarLogin/>
    </div>
  </template>

<script>
    import NavBarLogin from '@/components/Navs/NavBarLogin.vue'
    
    export default {
      name: 'Home',
      components: {NavBarLogin}
    }
    </script>