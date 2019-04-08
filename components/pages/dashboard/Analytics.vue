<template>
    <div class="section">
        <div class="column is-full">
            <div class="box is-fullwidth">
                <div class="columns is-full">
                    <div class="column is-half">
                        <h3 style="color: rgb(90,80,80); font-size:20px; font-weight: bold">Summary</h3>
                        <!-- <apexchart type=pie width=380 :options="chartOptions" :series="series" /> -->
                        <div class="column is-full">
                            <img src="@/assets/summary.jpg">
                        </div>
                    </div>
                    <div class="column is-half">
                        <h3 style="color: rgb(90,80,80); font-size:20px; font-weight: bold">Keuntungan : <span style="font-weight:normal;">Rp. 10.000.000,-</span></h3>
                        <br>
                        <h3 style="color: rgb(90,80,80); font-size:20px; font-weight: bold">Rekomendasi</h3>
                        <h3 style="color: rgb(90,80,80); font-size:14px; font-weight: normal">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</h3>
                    </div>
                </div>
            </div>
        </div>
        <div class="column is-full">
            <div class="columns">
                <div class="column is-half">
                    <div class="box is-fullwidth">
                        <h3 style="color: rgb(90,80,80); font-size:20px; font-weight: bold; margin-bottom: 20px;">Pemasukan</h3>
                        <img src="@/assets/income.jpg">
                        <br>
                        <br>
                        <table class="table is-striped is-hoverable">
                                    <thead>
                                    <tr style="background-color: #506cb5;">
                                        <th style="color: white;">Nama Barang</th>
                                        <th style="color: white;">Jumlah</th>
                                        <th style="color: white;">Harga</th>
                                    </tr>
                                    </thead>
                                    <tbody>
                                    <tr>
                                        <td>Nama barang 1</td>
                                        <td>10</td>
                                        <td>Rp100.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 2</td>
                                        <td>20</td>
                                        <td>Rp200.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 3</td>
                                        <td>30</td>
                                        <td>Rp300.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 4</td>
                                        <td>40</td>
                                        <td>Rp400.000,-</td>
                                    </tr>
                                    </tbody>
                                </table>
                    </div>
                </div>
                <div class="column is-half">
                    <div class="box is-fullwidth">
                        <h3 style="color: rgb(90,80,80); font-size:20px; font-weight: bold; margin-bottom: 20px;">Pengeluaran</h3>
                        <img src="@/assets/outcome.jpg">
                        <br>
                        <br>
                        <table class="table is-striped is-hoverable">
                                    <thead>
                                    <tr style="background-color: #506cb5;">
                                        <th style="color: white;">Nama Barang</th>
                                        <th style="color: white;">Jumlah</th>
                                        <th style="color: white;">Harga</th>
                                    </tr>
                                    </thead>
                                    <tbody>
                                    <tr>
                                        <td>Nama barang 1</td>
                                        <td>10</td>
                                        <td>Rp100.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 2</td>
                                        <td>20</td>
                                        <td>Rp200.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 3</td>
                                        <td>30</td>
                                        <td>Rp300.000,-</td>
                                    </tr>
                                    <tr>
                                        <td>Nama barang 4</td>
                                        <td>40</td>
                                        <td>Rp400.000,-</td>
                                    </tr>
                                    </tbody>
                                </table>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import ApexCharts from 'apexcharts';
    export default {
        components: {ApexCharts},
    }       
      /*  computed: {
            items() {
                return this.$store.state.items
            }
        }*/
    
</script>

<style>
    .section {
        padding: 24px;
    }
    @media (max-width: 768px) {
        .section {
            padding: 20px;
        }
    }
    @media (max-width: 414px) {
        .section {
            padding: 10px;
        }
    }
</style>