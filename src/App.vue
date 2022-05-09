<template>
  <h1>Staima</h1>
  <input type="text" name="email" v-model="email" /> <br />
  <input type="text" name="password" v-model="password" /> <br />
  <button v-on:click="addUser()">Add New User</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      email: "",
      password: "",
    };
  },
  methods: {
    addUser() {
      console.warn("function called",this.email,this.password);
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
