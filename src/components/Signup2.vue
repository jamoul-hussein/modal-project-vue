<template>
  <div class="container">
    <div class="form_container">
      <div class="title"><span>Login Form</span></div>
      <form action="#">
        <div class="row">
          <i class="fas fa-user"></i>
          <input type="text" placeholder="Email or Phone" required>
        </div>
        <div class="row">
          <i class="fas fa-lock"></i>
          <input type="password" placeholder="Password" required>
        </div>
        <div class="pass"><a href="#">Forgot password?</a></div>
        <div class="row button">
          <input type="submit" value="Login">
        </div>
        <div class="signup-link">Not a member? <a href="#">Signup now</a></div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "SignUp2",
  props: ["signupHeader"],
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: arial,sans-serif;
}
body{
  background: rgba(81, 30, 159, 0.39);
}

.container{
  max-width: 440px;
  padding: 0 20px;
  margin: 170px auto;
}

.form_container{
  width: 100%;
  background: #fff;
  border-radius: 5px;
  box-shadow: 0px 4px 10px 1px rgba(0,0,0,0.1);
}
.form_container .title{
  height: 90px;
  background: #16a085;
  border-radius: 5px 5px 0 0;
  color: #fff;
  font-size: 30px;
  font-weight: 600;
  display: flex;
  align-items: center;
  justify-content: center;
}
.form_container form{
  padding: 30px 25px 25px 25px;
}
.form_container form .row{
  height: 45px;
  margin-bottom: 15px;
  position: relative;
}
.form_container form .row input{
  height: 100%;
  width: 100%;
  outline: none;
  padding-left: 60px;
  border-radius: 5px;
  border: 1px solid lightgrey;
  font-size: 16px;
  transition: all 0.3s ease;
}
form .row input:focus{
  border-color: #16a085;
  box-shadow: inset 0px 0px 2px 2px rgba(26,188,156,0.25);
}
form .row input::placeholder{
  color: #999;
}
.form_container form .row i{
  position: absolute;
  width: 47px;
  height: 100%;
  color: #fff;
  font-size: 18px;
  background: #16a085;
  border: 1px solid #16a085;
  border-radius: 5px 0 0 5px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.form_container form .pass{
  margin: -8px 0 20px 0;
}
.form_container form .pass a{
  color: #16a085;
  font-size: 17px;
  text-decoration: none;
}
.form_container form .pass a:hover{
  text-decoration: underline;
}
.form_container form .button input{
  color: #fff;
  font-size: 20px;
  font-weight: 500;
  padding-left: 0px;
  background: #16a085;
  border: 1px solid #16a085;
  cursor: pointer;
}
form .button input:hover{
  background: #12876f;
}
.form_container form .signup-link{
  text-align: center;
  margin-top: 20px;
  font-size: 17px;
}
.form_container form .signup-link a{
  color: #16a085;
  text-decoration: none;
}
form .signup-link a:hover{
  text-decoration: underline;
}
</style>