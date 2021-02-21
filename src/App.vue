<template>
  <div id="app">
    <b-navbar
      toggleable="lg"
      type="dark"
      variant="dark"
      class="navbar-horizontal"
    >
      <b-navbar-brand href="#"
        ><h2><b-icon icon="emoji-dizzy-fill"></b-icon> <b>Tarot Card Shop</b> </h2>
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    </b-navbar>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #ff0000;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

</style>
