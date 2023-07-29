<template>
  <SignUp :signup-header="header"/>
</template>

<script>
import Modal from "./components/Modal.vue";
import SignUp from "./components/Signup.vue";

export default {
  name: "App",
  components: {
    Modal,
    SignUp,
  },
  data() {
    return {
      title: "",
      header: "Sign Up",
      text: "some text for sign up",
      theme: "sale",
      showPopUp: false,
    };
  },
  methods: {
    handleClick() {
      console.log(this.$refs.name);
      this.$refs.name.classList.add("active");
      this.$refs.name.focus();
    },
    toggle() {
      this.showPopUp = !this.showPopUp
    }
  },
};
</script>

<style>

/*#app {*/
/*  font-family: Avenir, Helvetica, Arial, sans-serif;*/
/*  -webkit-font-smoothing: antialiased;*/
/*  -moz-osx-font-smoothing: grayscale;*/
/*  text-align: center;*/
/*  color: #2c3e50;*/
/*  margin-top: 60px;*/
/*}*/
/*.buttonToggle {*/
/*  margin-top: 160px;*/
/*}*/
</style>
