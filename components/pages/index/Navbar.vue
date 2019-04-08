<template>
    <nav class="navbar is-transparent" style="padding-top: 0">
        <div class="container">
            <div class="navbar-brand">
                <a class="navbar-item" href="" style="padding: 0; margin-left: 0;">
                    <img src="~/assets/navbar-logo.png" class="logo" style="min-height: 7vh">
                </a>
                 <span class="navbar-burger burger has-text-white" data-target="navbarMenu" @click="activeBurger = !activeBurger" :class="{'is-active': activeBurger}">
                    <span></span>
                    <span></span>
                    <span></span>
                </span>
            </div>
            <div id="navbarMenu" class="navbar-menu" :class="{'is-active': activeBurger}">
                <div class="navbar-start">
                    <a class="navbar-item">
                        Home
                    </a>
                    <a class="navbar-item">
                        Tentang
                    </a>
                    <a class="navbar-item">
                        Layanan
                    </a>
                    <a class="navbar-item">
                        Kontak
                    </a>
                </div>
                <div class="navbar-end">
                    <div class="navbar-item" style="margin-right: 0">
                        <a class="button is-inverted is-info is-outlined" style="margin: 20px">
                            <nuxt-link to="/login" tag="span">Masuk</nuxt-link>
                        </a>
                        <a class="button is-outlined is-info is-inverted" style="margin: 20px">
                            <nuxt-link to="/signup" tag="span">Daftar</nuxt-link>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
  export default {
    name: 'Navbar',
    data() {
      return {
        'activeBurger': false
      }
    }
  }
</script>

<style scoped>
  .navbar {
    padding: 1% 9%;
    background-color: transparent;
  }
  .button {
    padding: 20px;
    border: 1px solid white;
  }
  .button:hover {
    border: 1px solid #27D2A3;
    background-color: #27D2A3;
  }
  .navbar-menu {
    background-color: transparent;
  }
  .navbar-item {
      margin: 0 20px;
  }
  .navbar-item:hover {
    background-color: transparent;
  }
  .navbar-item a {
    background-color: transparent;
    color: white;
  }
  .navbar-item a.is-active {
    color: white;
  }
  #daftar:hover {
    border-bottom: 1px solid white;
  }
  @media(max-width: 768px) {
    .navbar {
      padding: 1% 2%;
      background-color: transparent;
    }
  }
  @media(max-width: 434px) {
    .logo {
      max-height: 20px;
    }
  }
</style>