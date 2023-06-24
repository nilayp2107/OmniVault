<template>
  <NavBar count=2 />
  <LoginForm />
</template>

<script>
import NavBar from './components/NavBar.vue'
import LoginForm from './components/LoginForm.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    LoginForm
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;
}
</style>
