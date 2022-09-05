<template>
  <div class="signup">
      <NavBarSignup/>
      <Login/>
  </div>
</template>

<script>
import NavBarSignup from '@/components/Navs/NavBarSignup.vue'
import Login from '@/components/Forms/LoginForm.vue'
  
export default {
  name: 'Home',
  components: {NavBarSignup, Login}
}
</script>