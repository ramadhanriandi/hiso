<template>
  <section class="">
    <div>
      <Header />
      <Step />
      <Feature />
      <HeroBottom />
      <Footer />
    </div>
  </section>
</template>

<script>
import Header from '@/components/pages/index/Header'
import Step from '@/components/pages/index/Step'
import Feature from '@/components/pages/index/Feature'
import HeroBottom from '@/components/pages/index/HeroBottom'
import Footer from '@/components/shared/Footer'

export default {
  components: {
    Header,
    Step,
    Feature,
    HeroBottom,
    Footer,
  }
}
</script>

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
} */
</style>
