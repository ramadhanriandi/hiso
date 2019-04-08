<template>
    <div class="section has-text-grey-dark">
        <div class="columns">
            <div class="column">
                <h2 style="color: rgb(90,80,80); font-size:24px">Lakukan <strong style="color: #7e72b1">pengaturan</strong> terkait pencarian investor</h2>
            </div>
        </div>
        <div class="columns is-multiline is-mobile">
            <Investment/>            
        </div>
    </div>
</template>

<script>
    import Investment from './Investment'
    export default {
        components: {Investment},
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