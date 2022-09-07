<template>
  <div class="signup">
      <NavBarAlt/>
      <LoginForm/>
  </div>
</template>

<script>
import NavBarAlt from '@/components/Navs/NavBarAlt.vue'
import LoginForm from '@/components/Forms/LoginForm.vue'
  
export default {
  name: 'Home',
  components: {NavBarAlt, LoginForm}
}
</script>