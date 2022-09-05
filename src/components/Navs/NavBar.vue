<template>
    <div class="navbar">
        <div class="company">
            <router-link to="/"><img src="@/assets/logo.png" alt="logo" class="logo"></router-link>
            <router-link to="/" class="name">Shade</router-link>
        </div>
        <div class="links">
            <router-link to="">Market</router-link>
            <router-link to="">Buy Cryptos</router-link>
            <router-link to="">NFTs</router-link>
            <router-link to="">About Us</router-link>
            <router-link to="">Help</router-link>
        </div>
        <div class="button">
        <router-link class="btn1" to="/SignUp">Sign up</router-link>
        <router-link class="btn2" to="/Login">Log in</router-link>
        </div>
    </div>
  </template>

<script>
    export default {
        data(){
            return {
            }
        }
    }
</script>

<style>
.navbar{
    display: flex;
    padding-top: 17px;
    padding-bottom: 17px;
    padding-left: 12rem;
    padding-right: 6rem;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 2px 4px 0 rgba(0,0,0,.2);
}
.logo{
    position: absolute;
    height: 32px;
    width: 32px;
}
.name{
    margin-left: 4rem;
    color: #000000;
    font-size: 2.5rem;
    text-shadow: 0 0 0.9px #000;
}
.links a{
    margin: 0 1.5rem;
    color: #000000;
    font-size: 1.5rem;
    text-shadow: 0 0 0.7px #000;
}
.btn1{
    margin: 2.5rem;
    padding: 0.8rem 2.7rem;
    border-radius: 1.3rem;
    border: 1px solid #000000;
    color: #000000;
    font-size: 1.6rem;
    transition: all 0.3s ease 0s;
    cursor: pointer;
}
.btn1:hover{
    background-color: #2EE59D;
    color: #fff;
    box-shadow: 0px 15px 20px rgba(46, 229, 157, 0.4);
}
.btn2{
    padding: 0.8rem 2.7rem;
    background: #000000;
    border-radius: 1.3rem;
    border: 1px solid #000000;
    color: #fff;
    font-size: 1.6rem;
}
</style>