<template>
    <div class="signup">
        <NavBarSignup/>
        <Signup/>
    </div>
  </template>

<script>
  import NavBarSignup from '@/components/Navs/NavBarSignup.vue'
  import Signup from '@/components/Forms/SignupForm.vue'
    
  export default {
    name: 'Home',
    components: {NavBarSignup, Signup}
  }
</script>