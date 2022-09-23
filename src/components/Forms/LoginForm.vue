<template>
    <div class="signup">
      <form action="">
        <div class="form">
          <h1 class="title">Log In</h1>
          <div class="email">
            <label>Email</label>
            <input type="text" placeholder="Enter Email" required />
          </div>
          <div class="password">
            <label>Password</label>
            <input type="password" placeholder="Enter Password" minlength="8" maxlength="18" required />
          </div>
          <div class="submit-btn">
            <button type="submit" class="btn">Log In</button>
          </div>
          <div class="not-register">
            <p>Don't have an account? <router-link to="/SignUp"><span>Get Started</span></router-link></p>
          </div>
          <div class="split-line"></div>
        </div>
      </form>
    </div>
  </template>

<script>
  export default {
    data() {
      return {
      }
    }
  } 
</script>

<style scoped>
  .form {
    padding: 20px;
    width:750px;
    height: 600px;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    border-radius:10px;
    box-shadow: 2px 1px 21px -9px rgba(0,0,0,0.38);
    }
  .title{
    font-size: 3rem;
    text-align: center;
  }
  .email{
  padding-top: 40px;
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
  .not-register{
    padding-top: 10px;
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