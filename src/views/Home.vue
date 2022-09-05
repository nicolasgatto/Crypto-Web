<template>
  <div class="home">
    <NavBar/>
    <Background/>
      <h1 class="text-header">Buy, Sell & <br> Trade <span>Cryptos</span></h1>
      <p class="text">Wolrd biggest platform to buy, sell and trade Cryptocurrencies and NFTs.</p>
      <router-link to="/SignUp" class="btn3">Get started</router-link>
  </div>
</template>

<script>
import NavBar from '@/components/Navs/NavBar.vue'
import Background from '@/components/landingBack.vue'

export default {
  name: 'Home',
  components: {NavBar, Background}
}
</script>

<style scoped>
.home{
  color: #fff;
}
.text-header{
  font-size: 7rem;
  color: #000;
  margin-top: 100px;
  margin-left: 15rem;
}
span{
  color: #000;
}
.text{
  color: #000;
  font-size: 1.6rem;
  margin-left: 15rem;
  padding-top: 5rem;
}
.btn3{
  position: absolute;
  padding: 1rem 2.7rem;
  border-radius: 1.3rem;
  border: 1px solid #000000;
  color: #000;
  background-color: #fff;
  box-shadow: 0px 10px 15px rgba(0, 0, 0, 0.1);
  text-transform: uppercase;
  font-family: 'Roboto', sans-serif;
  font-size: 1.6rem;
  letter-spacing: 2.5px;
  margin-left: 30rem;
  margin-top: 130px;
  transition: all 0.3s ease 0s;
  cursor: pointer;
}
.btn3:hover {
  background-color: #2EE59D;
  box-shadow: 0px 15px 20px rgba(46, 229, 157, 0.4);
  color: #fff;
  transform: translateY(-7px);
}
  </style>