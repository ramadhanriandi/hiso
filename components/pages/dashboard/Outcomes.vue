<template>
    <div class="section has-text-grey-dark">
        <div class="columns">
            <div class="column">
                <h2 style="color: rgb(90,80,80); font-size:24px">Catat <strong style="color: #7e72b1">pengeluaran</strong> yang dilakukan</h2>
            </div>
            <div class="column is-one-sixths">
                <div class="is-pulled-right">
                    <a class="button" style="background-color: #7e72b1; color: white; padding:20px">Edit Kategori</a>
                    <a class="button" style="background-color: #506cb5; color: white; padding:20px">Reset</a>
                </div>
            </div>
        </div>
        <div class="columns is-multiline is-mobile">
            <Outcome/>            
        </div>
    </div>
</template>

<script>
    import Outcome from './Outcome'
    export default {
        components: {Outcome},
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