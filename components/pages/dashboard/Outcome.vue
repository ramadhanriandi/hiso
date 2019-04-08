<template>
    <div style="margin-top: 20px;">
        <div class="column is-full">
          <table class="table is-striped is-hoverable" style="width: 120%">
            <thead>
              <tr style="background-color: #506cb5;">
                <th style="color: white;">Nama Barang</th>
                <th style="color: white;">Jumlah</th>
                <th style="color: white;">Harga</th>
                <th style="color: white;">Kategori</th>
                <th style="color: white;">Keterangan</th>
                <th style="color: white;"></th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Nama barang 1</td>
                <td>10</td>
                <td>Rp100.000,-</td>
                <td>Nama kategori 1</td>
                <td>-</td>
                <td><span class="icon is-small"><i class="fas fa-times"></i></span></td>
              </tr>
              <tr>
                <td>Nama barang 2</td>
                <td>20</td>
                <td>Rp200.000,-</td>
                <td>Nama kategori 2</td>
                <td>-</td>
                <td><span class="icon is-small"><i class="fas fa-times"></i></span></td>
              </tr>
              <tr>
                <td>Nama barang 3</td>
                <td>30</td>
                <td>Rp300.000,-</td>
                <td>Nama kategori 3</td>
                <td>-</td>
                <td><span class="icon is-small"><i class="fas fa-times"></i></span></td>
              </tr>
              <tr>
                <td>Nama barang 4</td>
                <td>40</td>
                <td>Rp400.000,-</td>
                <td>Nama kategori 4</td>
                <td>-</td>
                <td><span class="icon is-small"><i class="fas fa-times"></i></span></td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="footer" style="width: 150%">
          <div class="columns is-vcentered">
            <div class="column is-4">
              <a class="button" style="background-color: #506cb5; color: white; padding:20px" onclick="handleTambahItem()">Tambah Item</a>
            </div>
            <div class="column" align="right">
              <div class="columns is-vcentered">
                <div class="column" align="right">
                  <p class="subtitle"><b>Total : Rp.400.000,-</b></p>
                </div>
                <div class="column" align="left">
                  <a class="button" style="background-color: #7e72b1; color: white; padding:20px">MASUKKAN</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
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