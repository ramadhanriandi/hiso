<template>
  <section class="header">
    <nav class="navbar is-transparent has-shadow is-fixed-top">
      <div class="navbar-brand">
        <a class="navbar-item" href="/">
          &nbsp &nbsp
          <img src="~/assets/navbar-logo.png">
        </a>
        <div role="button" class="navbar-burger burger" data-target="navMenu" style="padding:0" @click="activeBurger = !activeBurger" :class="{'is-active': activeBurger}">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <div class="navbar-menu">
        <div class="navbar-end is-hidden-mobile">
            <div class="navbar-item has-dropdown is-hoverable">
                <a class="navbar-link">
                Nama Pemilik
                </a>

                <div class="navbar-dropdown">
                    <a class="navbar-item">
                        Logout
                    </a>
                </div>
            </div>
        </div>
          <!-- <div class="navbar-item has-dropdown is-hoverable" v-if="selectedStore">
            <a class="navbar-link">
              {{ (selectedStore) ? selectedStore.name : stores[0].name }}
            </a>
            <div class="navbar-dropdown is-right">
              <a class="navbar-item has-icons-left" v-for="store in stores" @click="selectedStore = store">
                <span class="icon is-medium">
                  <fa :icon="['fas','shopping-bag']" class="has-text-white"/>
                </span>
                &nbsp &nbsp {{ store.name }}
              </a>
              <nuxt-link to="/dashboard/store/add" class="navbar-item has-icons-left">
                <span class="icon is-medium">
                  <fa :icon="['fas','plus']" class="has-text-white"/>
                </span>
                &nbsp &nbsp Tambah Toko
              </nuxt-link>
            </div>
          </div> -->
        </div>
      </div>
      <!-- 
      <div id="navmenu" class="navbar-menu is-hidden-tablet" :class="{'is-active': activeBurger}">
        <nav class="menu">
          <ul class="menu-list has-icons-left">
            <li>
              <a active-class="is-active" v-for="store in stores" @click="selectedStore = store">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','shopping-bag']" class="has-text-white"/>
                </span>
                &nbsp &nbsp {{ store.name }}
              </a>
            </li>
            <li>
              <nuxt-link to="/dashboard/store/add">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','plus']" class="has-text-white"/>
                </span>
                &nbsp &nbsp Tambah Toko
              </nuxt-link>
            </li>
            <hr class="underline">
            <li>
              <nuxt-link to="/dashboard" exact active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','shopping-cart']" />
                </span>
                &nbsp &nbsp &nbsp Items
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/order" exact active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','list']" />
                </span>
                &nbsp &nbsp &nbsp Order
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/features" active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','th']" />
                </span>
                &nbsp &nbsp &nbsp Features
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/analytics" active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','chart-bar']" />
                </span>
                &nbsp &nbsp &nbsp Analytics
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/settings" active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','cogs']" />
                </span>
                &nbsp &nbsp &nbsp Settings
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/deployment" active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','rocket']" />
                </span>
                &nbsp &nbsp &nbsp Deployment
              </nuxt-link>
            </li>
            <li>
              <nuxt-link to="/dashboard/access" active-class="is-active">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','address-card']" />
                </span>
                &nbsp &nbsp &nbsp Add access
              </nuxt-link>
            </li>
            <li>
              <a @click.prevent="handleLogout">
                <span class="icon is-small is-left">
                  <fa :icon="['fas','sign-out-alt']" />
                </span>
                &nbsp &nbsp &nbsp Log out
              </a>
            </li>
          </ul>
        </nav>
      </div> -->
    </nav>
  </section> 
</template>

<script>
  export default {
    name: 'Header',
    // data() {
    //   return {
    //     "activeBurger": false
    //   }
    // },
    // computed: {
    //   stores() {
    //     return this.$store.state.stores
    //   },
    //   selectedStore() {
    //     return this.$store.state.selected_store
    //   }
    // }
  }
</script>

<style scoped>
  .navbar {
    background-color: #F8F8F8;
    border-bottom: 1px solid #E7E7E7;
  }
  .navbar-item, .navbar-link {  
    background-color: transparent;
  }
  .navbar-dropdown {
    background-color: #7e72b1;
  }
  .navbar-dropdown .navbar-item {
    color: white;
  }
  a.navbar-item:hover, .navbar-link:hover {
    color: #7e72b1;
  }
  a.navbar-item.is-active, .navbar-link.is-active {
    color: #7e72b1;
  }
  .navbar-burger {
    background-color: transparent;
  }
  .navbar-menu {
    padding: 0.5rem 1rem 0.5rem 1rem;
  }     
  .menu-label {
    padding: 5px 0 5px 0;
    color: rgb(250, 250, 250);
  }
  .underline {
    display: block;
    height: 1px;
    border: 0;
    border-top: 1px solid;
    margin: 10px 0;
    padding: 0;
    color: rgb(200, 200, 200);
  }
  .menu-list {
    font-size: 15px;
  }
  .menu-list a {
    color: rgb(200, 200, 200);
    margin: 10px 0;
  }
  .menu-list a:hover {
    opacity: 10%;
    color: #7e72b1;;
  }
  .menu-list a.is-active {
    background: rgba(0, 0, 0, 0.1);
    color: white;
  }
</style>