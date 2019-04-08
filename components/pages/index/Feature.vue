<template>
  <div class="section category" style="padding-top:0">
    <div class="columns is-centered">
      <div class="header">
        <p class="subtitle has-text-centered" id="description">
          Nikmati berbagai <span id="emphasize"><b>fasilitas</b></span> di sini
        </p>
      </div>
    </div>
    <div class="columns is-centered is-variable is-5">
      <div class="column is-3">
        <div class="box">
          <div class="media-content">
            <div class="media" align="center">
                <img src="~/assets/facility_1.png" class="facility-pict">
            </div>
            <div class="content"> 
              <p class="title" align="center" style="margin: 10px; color: #506cb5;">Pencatatan<br>Keuangan</p>
              <p class="subtitle" align="center">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Phasellus nec iaculis mauris. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
            </div>
          </div>
        </div>
      </div>
      <div class="column is-3" style="margin-left: 50px; margin-right: 50px;">
        <div class="box">
          <div class="media-content">
            <div class="media" align="center">
                <img src="~/assets/facility_2.png" class="facility-pict">
            </div>
            <div class="content"> 
              <p class="title" align="center" style="margin: 10px; color: #506cb5;">Analisis dan<br>Rekomendasi</p>
              <p class="subtitle" align="center">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Phasellus nec iaculis mauris. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
            </div>
          </div>
        </div>
      </div>
      <div class="column is-3">
        <div class="box">
          <div class="media-content">
            <div class="media" align="center">
                <img src="~/assets/facility_3.png" class="facility-pict">
            </div>
            <div class="content"> 
              <p class="title" align="center" style="margin: 10px; color: #506cb5;">Investasi<br>Peer-to-peer</p>
              <p class="subtitle" align="center">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Phasellus nec iaculis mauris. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Feature'
  }
</script>

<style scoped>
  .container {
    padding: 3% 5%;
  }
  .title {
    color: rgb(80,80,90);
    font-size: 24px;
    font-weight: bold;
    line-height: 1.3;
    letter-spacing: 0px;
    padding-bottom: 20px;
  }
  .subtitle {
    font-size: 14px;
    line-height: 1.6;
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