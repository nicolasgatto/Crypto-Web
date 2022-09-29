<template>
  <div class="home">
    <NavBar/>
    <Landing/>
  </div>
</template>

<script>
import NavBar from '@/components/Navs/NavBar.vue'
import Landing from '@/components/landingPage.vue'

export default {
  name: 'Home',
  components: { NavBar, Landing}
}
</script>

<style scoped>

</style>