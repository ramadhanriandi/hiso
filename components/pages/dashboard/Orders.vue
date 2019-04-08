<template>
    <div class="section has-text-grey-dark">
        <div class="columns">
            <div class="column">
                <h2 style="color: rgb(90,80,80); font-size:24px">Pilih <strong style="color: #7e72b1">menu</strong> yang dibeli pelanggan</h2>
            </div>
            <div class="column is-one-fifths">
                <div class="is-pulled-right">
                    <a class="button" style="background-color: #7e72b1; color: white; padding:20px">Tambah Item</a>
                    <a class="button" style="background-color: #506cb5; color: white; padding:20px">Reset</a>
                </div>
            </div>
        </div>
        <div class="columns is-multiline is-mobile">
            <Order/>            
        </div>
    </div>
</template>

<script>
    import Order from './Order'
    export default {
        components: {Order},
      /*  computed: {
            items() {
                return this.$store.state.items
            }
        }*/
    }       
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