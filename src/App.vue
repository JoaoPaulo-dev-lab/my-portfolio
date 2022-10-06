<template>
    <div>
      <HeaderApp/>
      <BannerApp/>
      <ContatosApp/>
      <AboutApp/>
      <ServicesApp/>
      <PortfolioApp/>
    </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'
import BannerApp from './components/BannerApp.vue'
import AboutApp from './components/AboutApp.vue'
import ServicesApp from './components/ServicesApp.vue'
import PortfolioApp from './components/PortfolioApp.vue'
import ContatosApp from './components/ContatosApp.vue'
import '@fortawesome/fontawesome-free/css/all.css'
import './css/app.css'

export default {
  name: 'App',
  components: {
    HeaderApp, BannerApp, AboutApp, ServicesApp, PortfolioApp, ContatosApp
  }
}
</script>

<style>
*{
 font-family: 'Poppins', sans-serif;
 margin: 0;
 padding: 0;
 box-sizing: border-box;
 text-decoration: none;
}

html, body{
  width: 100%;
  height: 100%;
}
</style>
