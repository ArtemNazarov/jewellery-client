<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <h1 class="navbar-logo h1">JEWELLERY</h1>
      </a>

      <a
        role="button"
        class="navbar-burger burger"
        :class="{ 'is-active': isBurgerActive }"
        @click="toggleBurger"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarMenu"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbarMenu" class="navbar-menu" :class="{ 'is-active': isBurgerActive }">
      <div class="navbar-start">
        <router-link to="/" class="navbar-item">Home</router-link>
        <router-link to="/about" class="navbar-item">About</router-link>
      </div>

      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-primary">
              <strong>Buy everything</strong>
            </a>
            <a class="button is-light"> Log in </a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      isBurgerActive: false,
    };
  },
  methods: {
    toggleBurger() {
      this.isBurgerActive = !this.isBurgerActive;
    }
  }
};
</script>

<style>
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

.navbar-logo {
  font-size: 24px;
  font-family: "Poppins", sans-serif;
  letter-spacing: 5px;
}

nav {
  padding: 30px;
}
</style>