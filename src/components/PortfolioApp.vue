<template>
  <section class="portfolio-app bg-accent2">
    <SectionTitle title="Portfolio" subtitle="My Projects" idNav="portfolio"/>
    <div class="container-portfolio flex wrap justify-between">
        <PortfolioSingle link="https://www.google.com" path="https://i.pinimg.com/originals/70/98/98/709898ad1c77ebfaf579ff99268324ee.png" title="Clone TikTok"/>
        <PortfolioSingle link="https://www.facebook.com" :path="img2" title="Clone TikTok"/>
        <PortfolioSingle path="https://i.pinimg.com/originals/70/98/98/709898ad1c77ebfaf579ff99268324ee.png" title="Clone TikTok"/>
        <PortfolioSingle path="https://i.pinimg.com/originals/70/98/98/709898ad1c77ebfaf579ff99268324ee.png" title="Clone TikTok"/>
    </div>
  </section>
</template>

<script>
import PortfolioSingle from './PortfolioSingle.vue'
import SectionTitle from './SectionTitle.vue'
import img2 from '../assets/images/img2.jpg'

export default {
    name: 'PortfolioApp',
    components: {PortfolioSingle, SectionTitle},
    data(){
        return{
            img2
        }
    }
}
</script>

<style>
    .portfolio-app{
        width: 100%;
        padding: 30px 3% 50px 3%;
    }

    .container-portfolio{
        margin-top: 30px;
    }

    
</style>