<template>
    <div class="signup">
      <form>
        <div class="form">
          <h1 class="title">Sign Up</h1>
          <label for="email">Email</label>
          <input type="text" placeholder="Enter Email" required />
          <label for="psw">Password</label>
          <input type="password" placeholder="Enter Password" minlength="8" maxlength="18" required />
          <p>By creating an account you agree to our <router-link to="" style="color:dodgerblue">Terms of Use</router-link></p>
          <div class="submit-btn">
            <button type="submit" class="btn">Sign Up</button>
          </div>
          <div class="alredy-registered">
            <p>Already have an account? <router-link to="/Login"><span>Log In</span></router-link></p>
          </div>
          <div class="split-line"></div>
        </div>
      </form>
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
.title{
  text-align: center;
}
.form {
  padding: 20px;
  width:500px;
  height: 410px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  border-radius:10px;
  box-shadow: 2px 1px 21px -9px rgba(0,0,0,0.38);
  }
input{
  width: 100%;
  padding: 15px;
  margin: 5px 0 30px;
  border: none;
  background: #f7f7f7;
	font-family: 'Telex', sans-serif;
}
input[type=text]:focus, input[type=password]:focus, input[type=phone]:focus, select:focus {
  background-color: #ddd;
  outline: none;
}
.btn{
  background-color: #fff;
  color: #000;
  padding: 14px 20px;
  margin: 8px 0;
  margin-top: 30px;
  border: none;
  width: 100%;
	font-size: 1.6rem;
	font-family: 'Telex', sans-serif;
	border-radius:10px;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.4);
  transition: all 0.3s ease 0s;
  cursor: pointer;
}
button:hover {
  background-color: #2EE59D;
  color: #fff;
  box-shadow: 0 0 15px rgba(46, 229, 157, 0.4);
}
.alredy-registered{
  margin-top: 15px;
  color: #000;
  text-align: center;
}
span{
  color: dodgerblue;
}
.split-line{
    margin: 32px auto;
    width: 100%;
    height: 1px;
    background: #ddd;
}
</style>