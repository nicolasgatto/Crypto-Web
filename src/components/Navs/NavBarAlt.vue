<template>
    <div class="container-fluid">
        <div class="navbar">
            <div class="company">
                <router-link to="/"><img src="@/assets/logo.png" alt="logo" class="logo"></router-link>
                <router-link to="/" class="name">Shade</router-link>
            </div>
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

<style scoped>
a{
    text-decoration: none;
}
.container-fluid{
    padding-left: 0;
    padding-right: 0;
}
.navbar{
    padding-top: 17px;
    padding-bottom: 17px;
    padding-left: 6rem;
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
</style>