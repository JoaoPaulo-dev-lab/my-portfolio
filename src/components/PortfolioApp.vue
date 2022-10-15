<template>
  <section class="portfolio-app bg-accent2">
    <SectionTitle title="Portfólio" subtitle="Meus Projetos" idNav="portfolio"/>
    <div class="container-portfolio flex wrap justify-between">
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/clone-amazon" :path="amazon" title="Clone Prime Video"/>
        <PortfolioSingle :path="lista" title="ToDoList"/>
        <PortfolioSingle :path="pizzaria" title="Peça sua pizza"/>
    </div>
  </section>
</template>

<script>
import PortfolioSingle from './PortfolioSingle.vue'
import SectionTitle from './SectionTitle.vue'
import amazon from '../assets/images/amazon.jpg'
import lista from '../assets/images/lista.png'
import pizzaria from '../assets/images/pizzaria.png'


export default {
    name: 'PortfolioApp',
    components: {PortfolioSingle, SectionTitle},
    data(){
        return{
            amazon, lista, pizzaria
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