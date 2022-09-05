<template>
    <div class="navbar">
        <div class="company">
            <router-link to="/"><img src="@/assets/logo.png" alt="logo" class="logo"></router-link>
            <router-link to="/" class="name">Shade</router-link>
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
    justify-content: space-between;
    align-items: center;
    padding-top: 17px;
    padding-bottom: 17px;
    padding-left: 12rem;
    padding-right: 6rem;
    box-shadow: 0 2px 4px 0 rgba(0,0,0,.2);
}
.logo{
    position: absolute;
    height: 32px;
    width: 32px;
}
.name{
    color: #000000;
    font-size: 2.5rem;
    margin-left: 4rem;
    text-shadow: 0 0 0.9px #000;
}
</style>