<template>
  <div class="container">

    <h1>Sign Up</h1>

    <label for="email" id="email_label">Email</label>
    <input type="text" placeholder="Enter Email" name="email" id="email">

    <label for="password" id="password_label">Password</label>
    <input type="password" placeholder="Enter Password" name="psw" id="password">

    <p>By creating an account you agree to our <a href="#">Terms & Privacy</a>.</p>
    <button type="submit" class="signup_btn">Sign Up</button>
  </div>
</template>

<script>
export default {
  name: "SignUp1",
  props: ["signupHeader"],
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  justify-items: center;
  align-content: center;
  text-align: center;
  /*margin: 250px 700px;*/
  border: rgba(0, 0, 0, 0.93) solid 2px;
  border-radius: 8px;
  height: 600px;
  width: 600px;
  box-shadow: rgba(0, 0, 0, 0.19) 10px 20px 40px,rgba(0, 0, 0, 0.19) 10px 20px 40px;
}

.container h1 {
  margin: 40px 0 39px 0;
  border: rgba(0, 0, 0, 0.19) solid 3px;
  border-left: none;
  border-right: none;
  width: 100%;
  background-color: rgba(31, 16, 16, 0.43);
  color: white;
}

.container #email{
  width: 90%;
  margin-bottom: 50px;
  border: rgba(0, 0, 0, 0.38) solid 2px;
  border-radius: 8px;
  padding: 10px;
}

.container #email_label {
  margin-bottom: 10px;
  font-weight: bold;
  font-size: 20px;
}

.container #password {
  width: 90%;
  margin-bottom: 50px;
  border: rgba(0, 0, 0, 0.38) solid 2px;
  border-radius: 8px;
  padding: 10px;
}

.container #password_label {
  margin-bottom: 10px;
  font-weight: bold;
  font-size: 20px;
}

.container p, a{
  font-size: 18px;
}

.container .signup_btn {
  margin-top: 25px;
  padding: 15px 40px;
  border: rgba(0, 0, 0, 0.19) solid 1px;
  border-radius: 8px;
  font-size: 18px;
  font-weight: bold;
  background-color: rgba(51, 0, 128, 0.39);
}
</style>