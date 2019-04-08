<template>
  <nav class="menu">
    <p class="menu-label">
      Dashboard
    </p>
    <hr class="underline">
    <ul class="menu-list has-icons-left">
      <li>
        <nuxt-link to="/dashboard" exact active-class="is-active">
          <span class="icon is-small is-left">
            <img src="@/assets/analytics.png">
          </span>
          &nbsp &nbsp &nbsp Analisis
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/dashboard/pemasukan" exact active-class="is-active">
          <span class="icon is-small is-left">
            <img src="@/assets/income.png">
          </span>
          &nbsp &nbsp &nbsp Pemasukan
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/dashboard/pengeluaran" active-class="is-active">
          <span class="icon is-small is-left">
            <img src="@/assets/outcome.png">
          </span>
          &nbsp &nbsp &nbsp Pengeluaran
        </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/dashboard/investasi" active-class="is-active">
          <span class="icon is-small is-left">
            <img src="@/assets/investation.png">
          </span>
          &nbsp &nbsp &nbsp Investasi
        </nuxt-link>
      </li>
    </ul>
    <p class="menu-label">
      SETTINGS
    </p>
    <hr class="underline">
    <ul class="menu-list has-icons-left">
      <li>
        <nuxt-link to="/dashboard/profil" active-class="is-active">
          <span class="icon is-small is-left">
            <img src="@/assets/profile.png">
          </span>
          &nbsp &nbsp &nbsp Profil
        </nuxt-link>
      </li>
      <!-- <li>
        <a @click.prevent="handleLogout">
          <span class="icon is-small is-left">
            <fa :icon="['fas','sign-out-alt']" />
          </span>
          &nbsp &nbsp &nbsp Log out
        </a>
      </li> -->
    </ul>
  </nav>
</template>

<script>
  export default {
    methods: {
      handleLogout() {
        this.$emit("onLogout");
      }
    }
  }
</script>
  
<style scoped>
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
    color:  #7e72b1;;
  }
  .menu-list a.is-active {
    background: rgba(0, 0, 0, 0.1);
    color: white;
  }
</style>