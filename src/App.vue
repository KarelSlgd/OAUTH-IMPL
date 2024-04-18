<template>
  <div class="app">
    <div class="nav">
      <router-link class="link" to="/">Home</router-link>|
      <router-link class="link" v-if="$auth.isAuthenticated" to="/profile"
        >Profile</router-link
      >
    </div>
    <router-view />
  </div>
</template>

<script>
export default {};
</script>

<style>
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
.nav {
  margin-bottom: 20px;
}
body {
  margin: 0;
  padding: 0;
  background-color: #dfdfdf;
}
.link {
  text-decoration: none;
  color: #000;
  font-size: 20px;
}
</style>