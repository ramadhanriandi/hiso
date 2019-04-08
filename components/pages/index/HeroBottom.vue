<template>
  <div class="section category" style="padding-top:5vh; padding-bottom:10vh;">
    <div class="columns is-centered">
      <div class="header">
        <p class="subtitle has-text-centered" id="description">
          atau mulai langkah <span id="emphasize"><b>Investasi</b></span> di sini
        </p>
      </div>
    </div>
    <div class="columns is-vcentered">
        <div class="column is-5 phone_img" data-aos="zoom-in">
            <div class="has-text-centered">
                <img src="~/assets/invest.png" align="right" alt="Atur Finansialmu dan Dapatkan Pendanaan" style="max-width: 60%; margin-right: 20px;">
            </div>
        </div>
        <div class="column is-5" style="margin-left: 20px;">
            <p class="subtitle is-6">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            </p>    
            <a class="button is-small is-rounded" style="background-color: #506cb5; color: white;"><nuxt-link to="/login" tag="span">MULAI INVESTASI</nuxt-link></a>
        </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'HeroBottom'
  }
</script>

<style scoped>
  .container {
    padding: 3% 5%;
  }
  .title {
    color: rgb(80,80,90);
    font-size: 42px;
    font-weight: bold;
    line-height: 1.3;
    margin-bottom: 30px;
    letter-spacing: 0px;
  }
  .subtitle {
    font-size: 16px;
    line-height: 2;
  }
  .button {
    margin-top: 10px;
    font-weight: bold;
    padding: 20px;
    font-size: 16px
  }
  #description {
    font-size: 28px;
    margin-bottom: 4vh;
  }
  #emphasize {
    color: #7e72b1;
    font-size: 42px;
  }
  .facility-pict {
    padding: 25px;
    padding-bottom: 10px;
  }
  @media(max-width: 768px) {
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
  }
</style>