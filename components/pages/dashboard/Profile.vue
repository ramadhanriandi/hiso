<template>
    <div class="column is-full">
        <div class="box">
          <div class="columns">
            <div class="column is-4">
              <p style="margin-bottom: 20px;">Nama Lengkap</p>
              <p style="margin-bottom: 20px;">Email</p>
              <p style="margin-bottom: 20px;">Nomor Handphone</p>
              <p style="margin-bottom: 20px;">Nomor Rekening</p>
              <p style="margin-bottom: 20px;">NPWP</p>
              <p style="margin-bottom: 20px;">Upload Foto Profil</p>
              <p>Upload KTP</p>
            </div>
            <div class="column">
              <input class="input" type="text" placeholder="Nama Lengkap" value="Muhammad Fariz Luthfan Wakan" style="margin-bottom: 5px;">
              <input class="input" type="email" disabled placeholder="Email" value="irluths@gmail.com" style="margin-bottom: 5px;">
              <input class="input" type="tel" placeholder="Nomor Handphone" value="08123456xxxx" style="margin-bottom: 5px;">
              <input class="input" type="text" placeholder="Nomor Rekening" value="214135xxxxxx" style="margin-bottom: 5px;">
              <input class="input" type="text" placeholder="NPWP" value="12931204xxxxxxx" style="margin-bottom: 5px;">
              <div class="file has-name is-fullwidth" style="margin-bottom: 5px;">
                <label class="file-label">
                  <input class="file-input" type="file" name="foto-profil">
                  <span class="file-cta">
                    <span class="file-icon">
                      <i class="fas fa-upload"></i>
                    </span>
                    <span class="file-label">
                      Upload Foto Profil
                    </span>
                  </span>
                  <span class="file-name">
                    Screen Shot 2017-07-29 at 15.54.25.png
                  </span>
                </label>
              </div>
              <div class="file has-name is-fullwidth" style="margin-bottom: 5px;">
                <label class="file-label">
                  <input class="file-input" type="file" name="ktp">
                  <span class="file-cta">
                    <span class="file-icon">
                      <i class="fas fa-upload"></i>
                    </span>
                    <span class="file-label">
                      Upload KTP
                    </span>
                  </span>
                  <span class="file-name">
                    Screen Shot 2017-07-29 at 15.54.25.png
                  </span>
                </label>
              </div>
            </div>
          </div>
          <hr>
          <div class="columns">
            <div class="column is-4">
              <p style="margin-bottom: 20px;">Nama Usaha</p>
              <p style="margin-bottom: 20px;">Deskripsi Usaha</p>
              <p style="margin-bottom: 20px;">Alamat Usaha</p>
            </div>
            <div class="column">
              <input class="input" type="text" placeholder="Nama Usaha" value="Warung Tenda Cisitu" style="margin-bottom: 5px;">
              <input class="input" type="text" placeholder="Deskripsi Usaha" value="Makanan harga mahasiswa" style="margin-bottom: 5px;">
              <input class="input" type="text" placeholder="Alamat Usaha" value="Jalan Cisitu Lama No. xx Kel. Dago Kec. Coblong Bandung" style="margin-bottom: 5px;">
            </div>
          </div>
        </div>
        <div class="column">
            <div class="is-pulled-right">
                <a class="button" style="padding:20px">BATAL</a>
                <a class="button" style="background-color: #506cb5; color: white; padding:20px">SIMPAN</a>
            </div>
        </div>
    </div>
</template>

<script>
 /*   export default {
        props: ['itemData']
    }       */
</script>

<style>
    .title {
        font-size: 24px;
    }
    .order-name {
        font-size: 24px;
        font-weight: bolder;
    }
    .sub-content {
        padding: 0 10px;
        line-height: 2;
    }
    #line-divider {
        margin: 10px 0;
    }
    .input {
        padding: 2vh;
    }
    @media (max-width: 694px) {
	    .title {
            font-size: 20px;
        }
        .order-name {
            font-size: 18px;
        }
    }
    @media (max-width: 414px) {
	    .title {
            font-size: 16px;
        }
    }
</style>