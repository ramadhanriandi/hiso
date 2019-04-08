<template>
    <div class="column is-full" style="margin-top: 20px;">
        <div class="field" style="margin-bottom: 5vh;">
            <input id="switchRoundedDefault" type="checkbox" name="switchRoundedDefault" class="switch is-rounded" checked="checked">
            <label for="switchRoundedDefault">Sedang mencari <strong>pendanaan</strong></label>
        </div>
        <div class="card" style="border-radius:5px">
            <div class="card-content is-fullwidth">
                <div class="field is-horizontal">
                    <div class="field-label is-normal">
                        <label class="label">Dana yang dibutuhkan</label>
                    </div>
                    <div class="field-body">
                        <div class="field is-expanded">
                            <div class="field has-addons">
                                <p class="control">
                                    <a class="button is-static">
                                        Rp.
                                    </a>
                                </p>
                                <p class="control">
                                    <input class="input" type="text">
                                </p>
                                <p class="control">
                                    <a class="button is-static">
                                        ,-
                                    </a>
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="field is-horizontal">
                    <div class="field-label is-normal">
                        <label class="label">Jangka waktu pencarian</label>
                    </div>
                    <div class="field-body">
                        <div class="field is-expanded">
                            <div class="field has-addons">
                                <p class="control">
                                    <input class="input" type="text">
                                </p>
                                <p class="control">
                                    <a class="button is-static">
                                        bulan
                                    </a>
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="field is-horizontal">
                    <div class="field-label is-normal">
                        <label class="label">Durasi investasi</label>
                    </div>
                    <div class="field-body">
                        <div class="field is-expanded">
                            <div class="field has-addons">
                                <p class="control">
                                    <input class="input" type="text">
                                </p>
                                <p class="control">
                                    <a class="button is-static">
                                        bulan
                                    </a>
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="column is-pulled-right" align="left">
            <a class="button" style="background-color: #7e72b1; color: white; padding:20px">Masukkan</a>
        </div>
    </div>

    <!--  MODAL TAMBAH ITEM  -->
    <!-- <div class="modal" id="tambah-item">
      <div class="modal-background" onclick="closeTambahItem()"></div>
      <div class="modal-card">
        <header class="modal-card-head">
          <p class="modal-card-title">Tambah Item</p>
          <button class="delete" aria-label="close" onclick="closeTambahItem()"></button>
        </header>
        <section class="modal-card-body">
          <input class="input" type="text" placeholder="Nama Barang" style="margin-bottom: 10px;">
          <input class="input" type="text" placeholder="Jumlah" style="margin-bottom: 10px;">
          <input class="input" type="text" placeholder="Harga" style="margin-bottom: 10px;">
          <div class="select is-rounded is-info" style="margin-bottom: 10px;">
            <select>
              <option>Kategori</option>
              <option>Kategori 1</option>
              <option>Kategori 2</option>
              <option>Kategori 3</option>
              <option>Kategori 4</option>
              <option>Kategori 5</option>
            </select>
          </div>
          <input class="input" type="text" placeholder="Keterangan" style="margin-bottom: 10px;">
          <!-- Content ... -->
        <!-- </section>
        <footer class="modal-card-foot">
          <button class="button is-success">Simpan</button>
          <button class="button" onclick="closeTambahItem()">Batal</button>
        </footer>
      </div>
    </div> -->
</template>

<script type="text/javascript">
    /* HANDLER TAMBAH ITEM */
    handleTambahItem = () => {
    document.getElementById('tambah-item').classList.add('is-active');
    }
    closeTambahItem = () => {
    document.getElementById('tambah-item').classList.remove('is-active');
    }   
</script>

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