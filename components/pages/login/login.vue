<template>
    <form @submit.prevent="$emit('handleLogin', {email, password})">
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
        <div class="is-pulled-right">
            <a href="" >Lupa password ?</a>
        </div>
        <br>
        <div class="has-text-centered">
            <nuxt-link to="dashboard" tag="span"><button type="submit" class="button is-vcentered is-link is-outlined">MASUK</button></nuxt-link>
        </div>
    </form>
</template>

<script>
    export default {
        name: 'Login',
        data() {
            return {
                email: '',
                password: ''
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