<template>
  <section class="bg-accent2 about">
    <SectionTitle title="Sobre mim" subtitle="Quem sou eu?" idNav="about"/>
    <div class="about-box flex justify-between">
        <div class="description flex column">
            <p class="text-description text-secundary">Meu nome é João Paulo Maciel. Sou desenvolvedor front-end e moro em Arcoverde, no estado de Pernambuco. Estou procurando uma oportunidade para começar minha carreira como desenvolvedor junior. Comecei meus estudos em programação no final de 2021 e decidi me dedicar à tecnologia em Abril de 2022, depois de me encantar com o desenvolvimento web. Todos os dias aprendo algo diferente e aprimoro minhas habilidades, seguindo dicas de desenvolvedores mais experientes. Estou disposto a aprender novas tecnologias e encarar desafios.</p>
            <div>
                <a href="https://my-portfolio-dev-a4a9c.web.app/curriculo.pdf" class="link-action bg-accent text-bold" download="curriculo.pdf">Baixar CV</a>
            </div>
        </div>
        <div class="skills bg-accent3 flex">
            <div class="skill-single">
                <Skill title="Html 5" :level="5"/>
            </div>
            <div class="skill-single">
                <Skill title="CSS 3" :level="3"/>
            </div>
             <div class="skill-single">
                <Skill title="JavaScript" :level="3"/>
            </div>
            <div class="skill-single">
                <Skill title="Vue JS" :level="3"/>
            </div>
            <div class="skill-single">
                <Skill title="Bootstrap" :level="2"/>
            </div>
            <div class="skill-single">
                <Skill title="Spectre" :level="2"/>
            </div>
            <div class="skill-single">
                <Skill title="Vuex" :level="2"/>
            </div>
            <div class="skill-single">
                <Skill title="Git" :level="3"/>
            </div>
            <div class="skill-single">
                <Skill title="TypeScript" :level="3"/>
            </div>
            
        </div>
    </div>
  </section>
</template>

<script>
import SectionTitle from './SectionTitle.vue'
import Skill from './Skill.vue'
export default {
    name: 'AboutApp',
    components: {
        SectionTitle, Skill
    }
}
</script>

<style>
    .about{
        width: 100%;
        padding: 30px 3% 50px 3%;
    }
    .about-box{
        width: 100%;
        margin-top: 15px;
        
    }

    .about-box .description{
        width: 48%;
    }

    .skills{
        width: 48%;
        padding: 20px 3%;
        flex-wrap: wrap;

    }

     .skills .skill-single{
        width: 33%;
    }

    @media screen and (max-width: 820px){
        .about-box{
        flex-wrap: wrap;
        
    }
        .about-box .description{
        width: 100%;
        margin-bottom: 30px;
    }

    .skills{
        width: 100%;

    }
    }

    @media screen and (max-width: 500px){
        .skills .skill-single{
        width: 50%;
        display: flex;
        justify-content: center;
        }
    }
</style>