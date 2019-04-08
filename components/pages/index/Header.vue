<template>
  <section class="hero is-fullheight " >
    <div class="hero-head">
      <Navbar />
    </div>
    <div class="hero-body">
      <div class="container">
        <div class="columns">
          <div class="column is-6-tablet is-full-mobile hero-text">
            <p class="title is-spaced" style="color: #506cb5;">
              Buat Bisnismu<br />Lebih Optimum
            </p>
            <p class="subtitle">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </p>
            <a class="button is-small is-rounded" style="background-color: #7e72b1; color: white;"><nuxt-link to="/login" tag="span">DAFTAR SEKARANG</nuxt-link></a>
          </div>
          <div class="column is-6-tablet has-text-right" >
            <img id="phone" src="~/assets/hero-picture.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  import Navbar from './Navbar'
  export default {
      name: 'Header',
      components: { Navbar }
  }
</script>

<style scoped>
  .hero {
    width: 100%;
    height: 100%;
    background-image: url(~assets/hero-background.png);
    background-size: cover;
  }
  .hero-body {
    padding: 0% 2.5%;
  }
  .container {
    padding: 3% 5%;
  }
  .title {
    color: white;
    font-size: 54px;
    font-weight: bold;
    line-height: 1.3;
    margin-bottom: 10px;
    letter-spacing: 0px;
  }
  .subtitle {
    font-size: 14px;
    line-height: 2;
  }
  .button {
    margin-top: 10px;
    font-weight: bold;
    padding: 20px;
    font-size: 16px
  }
  #phone {
      max-width: 450px;
  }
  @media(max-width: 768px) {
    #phone {
      max-height: 45vh;
    }
  }
  @media(max-width: 434px) {
    .hero-body {
      padding: 0% 2.5%;
    }
    .title {
      font-size: 36px;
      margin-bottom: 10px;
    }
    .subtitle {
      font-size: 12px;
    }
    .button {
      margin-top: 0px;
      padding: 15px 25px;
      font-size: 16px;
    }
    #phone {
      max-height: 38vh;
    }
  }
</style>

<style unscoped>
  @import url('https://fonts.googleapis.com/css?family=Quicksand:300,400,500,700');
  body {
	  font-family: 'Quicksand', sans-serif;
    color: rgb(80,80,90);
    letter-spacing: 0.5px;
    font-weight: 400;
  }
</style>