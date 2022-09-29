<template>
    <div class="signup">
        <NavBar/>
        <CoinsPrice/>
    </div>
  </template>

<script>
  import NavBar from '@/components/Navs/NavBar.vue'
  import CoinsPrice from '@/components/Market/CoinsPrices.vue'
  
  export default {
    name: 'Home',
    components: { NavBar, CoinsPrice}
  }
</script>