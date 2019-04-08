<template>
    <form @submit.prevent="$emit('handleRegistration', {email})">
        <div class="field">
            <label class="label"><b>Nama Lengkap</b></label>
            <div class="control has-icons-right">
                <input class="input" type="text" v-model="email">
                <span class="icon is-small is-right">
                    <fa :icon="['fas','envelope']" />
                </span>
            </div>
        </div>
        <div class="field">
            <label class="label"><b>E-mail</b></label>
            <div class="control has-icons-right">
                <input class="input" type="text" v-model="email">
                <span class="icon is-small is-right">
                    <fa :icon="['fas','envelope']" />
                </span>
            </div>
        </div>
        <div class="field">
            <label class="label">Password</label>
            <div class="control has-icons-right">
                <input class="input" type="password" v-model="password">
                <span class="icon is-small is-right">
                    <fa :icon="['fas','key']" />
                </span>
            </div>
        </div>
        <div class="field">
            <label class="label">No. Handphone</label>
            <div class="control has-icons-right">
                <input class="input" type="password" v-model="password">
                <span class="icon is-small is-right">
                    <fa :icon="['fas','key']" />
                </span>
            </div>
        </div>
        <div class="is-pulled-left">
            <label class="checkbox">
                <p style="font-size: 10px"><input type="checkbox">&nbsp Saya setuju dengan <a href="" style="color:#7e72b1; font-weight: bolder;">syarat dan ketentuan</a> yang berlaku</p>
            </label>
        </div>
        <br>
        <br>
        <div class="has-text-centered">
            <button type="submit" class="button is-vcentered is-fullwidth" style="background-color: #506cb5; color: white; font-weight: bolder">Daftar sebagai Pemilik Usaha</button>
        </div>
        <div class="has-text-centered">
            atau
        </div>
        <div class="has-text-centered">
            <button type="submit" class="button is-vcentered is-fullwidth" style="background-color: #506cb5; color: white; font-weight: bolder">Daftar sebagai Investor</button>
        </div>
    </form>
</template>

<script>
    export default {
        name: 'New',
        data() {
            return {
                email: ''
            }
        }
    }
</script>

<style scoped>
    .input {
        border-radius: 50px;
    }
    .button {
        margin-top: 20px;
        margin-bottom: 20px;
        min-width: 150px;
    }
</style>