<template>
    <div class="signup">
        <NavBarAlt/>
        <SignupForm/>
    </div>
  </template>

<script>
  import NavBarAlt from '@/components/Navs/NavBarAlt.vue'
  import SignupForm from '@/components/Forms/SignupForm.vue'
    
  export default {
    name: 'Home',
    components: {NavBarAlt, SignupForm}
  }
</script>