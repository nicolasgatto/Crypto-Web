<template>
    <div class="signup">
        <NavBarSignup/>
        <h1 class="title">Get Started</h1>
    </div>
  </template>

<script>
    import NavBarSignup from '@/components/Navs/NavBarSignup.vue'
    
    export default {
      name: 'Home',
      components: {NavBarSignup}
    }
</script>

<style>
.title{
    text-align: center;
    color: #000000;
    font-size: 3.5rem;
    margin: 0 1.5rem;
    text-shadow: 0 0 0.7px #000;
    font-weight: 400;
    margin-top: 70px;
}
</style>