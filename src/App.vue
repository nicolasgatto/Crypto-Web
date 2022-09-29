<template>
  <div class="App">
    <router-view v-slot="{ Component }">
      <transition name="fade" mode="out-in">
        <component :is="Component" />
      </transition>
    </router-view>
  </div>
</template>

<script>
  export default {
    name: 'Home',
    components: {}
  }
  </script>

<style>
.fade-enter-from,
.fade-leave-to {
  opacity: 0
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.6s ease-out;
}
</style>