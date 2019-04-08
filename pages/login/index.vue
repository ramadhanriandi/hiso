<template>
  <div class="hero container-fluid gradient is-full">
    <div class="column is-vcentered">
      <div class="login is-hcentered is-vcentered column is-4 is-offset-4">
        <section class="section interactive-bg"> 
          <div class="has-text-centered">
            <a href="/"><img class="login-logo" src="~/assets/navbar-logo.png"></a>
          </div>
          <Notification :message="error" type="error" v-if="error"/>
          <Notification :message="success" type="success" v-if="success"/>  
          <Login/>
          <hr class="is-full-width">   
          <div class="has-text-grey has-text-centered">
            <p>
              Belum punya akun ? 
              <nuxt-link to="login" tag="span"><a>Daftar</a></nuxt-link>
            </p>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
  import Notification from '@/components/shared/Notification'
  import Login from '@/components/pages/login/login'

  export default {
    components: { Notification, Login},
  //  middleware: ['init','auth-dashboard'],
    // data() {
    //   return {
    //     view: 'Login',
    //     error: null,
    //     success: null   
    //   }
    // },
    // methods: {
    //   login(e) {
    //     this.$store.dispatch('authenticateUser', {
    //       email: e.email,
    //       password: e.password,
    //     })
    //     .then(() => {
    //       this.$router.push('/dashboard')
    //     })
    //     .catch((e) => {
    //       this.error = e.response.data.msg
    //     })
    //   },    
    // }
  }
</script>

<style unscoped>
  @import url('https://fonts.googleapis.com/css?family=Quicksand:300,400,500,700');
  body {
	  font-family: 'Quicksand', sans-serif;
    color: rgb(90, 80, 80);
    letter-spacing: 0.5px;
    font-weight: 400;
  }
  .label {
    font-weight: bold;
  }
  .container-fluid {
	  padding: 8vh 0 8vh 0;
  }
  .gradient {
	  width: 100%;
	  height: 100%;
	  background-color: #efefef;
  }
  .interactive-bg {
  	height: auto;
  	width:100%;
  	appearance: none;
	  border-radius: 10px;
	  display: block;
	  background-color: white;
	  transition-duration: 0.25s;
	  font-weight: 300;
  }
  .login-logo {
    margin: 0 auto;
    margin-bottom: 25px;
    max-height: 100px;
  }
  hr {    
    margin:0 0 10px 0;
    height:1px;
    background:#c9cdd3;
  }
  @media (max-width: 768px) {
	  .container-fluid {
		  padding: 12vh;	
    }
    .login {
      height: auto;
    }
    .column {
		  padding: 0;
    }
    .interactive-bg {
	  	border-radius: 10px;
	  }
  }
  @media (max-width: 414px) {
	  .container-fluid {
		  padding: 0;	
    }
    .gradient {
		  height: 100%;
    }
    .login {
		  height: auto;
    }
    .column {
		  padding: 0;
    }
    .interactive-bg {
	  	border-radius: 0px;
	  }
  }
</style>