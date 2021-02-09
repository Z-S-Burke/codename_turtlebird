<template>
  <div id="app">
    <b-navbar class="header_style" toggleable="lg" top="fixed" id="navbar">
      <b-navbar-brand>
        <router-link to="/" class="d-flex align-items-center-text-light ml-2">
          <h2 class="ml-2 mt-2 text-dark">Brent Jones</h2>
        </router-link>
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" class="navItems"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item>
            <router-link class="text-dark" to="/">Home</router-link>
          </b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav>
          <b-nav-item>
            <router-link class="text-dark" to="/bio">R&amp;D</router-link>
          </b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav>
          <b-nav-item>
            <router-link class="text-dark" to="/CV">CV</router-link>
          </b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav>
          <b-nav-item>
            <router-link class="text-dark" to="/Blog">Blog</router-link>
          </b-nav-item>
        </b-navbar-nav>

        <b-navbar-nav>
          <b-nav-item>
            <router-link class="text-dark" to="/contact">Contact</router-link>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>


<style scoped>
.logo {
  height: 50px;
  width: 50px;
}

.header_style {
  background-color: #66bb6a;
  border-top: solid #338a3e 25px;
}

.navItems {
    background-color: #2196f3;
    border: solid white 1px;
}

.logo_text {
  text-decoration: none;
}
.custom_bg_color {
  background-color: rgb(241, 144, 16);
}
</style> 