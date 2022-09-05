<template>
  <div class="App">
    <transition name="fade" mode="out-in">
      <router-view/>
    </transition>
    <Footer/>
  </div>
</template>

<script>
import Footer from '@/components/Footer.vue'
  
  export default {
    name: 'Home',
    components: {Footer}
  }
  </script>

<style>
.fade-enter-active,
.fade-leave-active {
  transition-duration: 0.5s;
  transition-property: opacity;
  transition-timing-function: ease;
}

.fade-enter,
.fade-leave-active {
  opacity: 0
}
</style>