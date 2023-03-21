<template>
  <section class="portfolio-app bg-accent2">
    <SectionTitle title="Portfólio" subtitle="Meus Projetos" idNav="portfolio"/>
    <div class="container-portfolio flex wrap justify-between">
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/clone-amazon" :path="amazon" title="Clone Prime Video"/>
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/to-do-list-router" :path="lista" title="ToDoList"/>
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/pizzaria" :path="pizzaria" title="Peça sua pizza"/>
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/form" :path="formulario" title="Formulário com Validação"/>
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/galeria-torcedor" :path="galeria" title="Galeria do Torcedor"/>
        <PortfolioSingle link="https://github.com/JoaoPaulo-dev-lab/controle-financeiro" :path="financeiro" title="Controle Financeiro"/>
    </div>
  </section>
</template>

<script>
import PortfolioSingle from './PortfolioSingle.vue'
import SectionTitle from './SectionTitle.vue'
import amazon from '../assets/images/amazon.jpg'
import lista from '../assets/images/lista.png'
import pizzaria from '../assets/images/pizzaria.png'
import formulario from '../assets/images/formulario.png'
import galeria from '../assets/images/galeria.png'
import financeiro from '../assets/images/controle-financeiro.png'


export default {
    name: 'PortfolioApp',
    components: {PortfolioSingle, SectionTitle},
    data(){
        return{
            amazon, lista, pizzaria, formulario, galeria, financeiro
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