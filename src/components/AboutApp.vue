<template>
  <section class="bg-accent2 about">
    <SectionTitle title="About Me" subtitle="Who am I" idNav="about"/>
    <div class="about-box flex justify-between">
        <div class="description flex column">
            <p class="text-description text-secundary">My name is João Paulo Maciel. I'm a front-end developer and live in Arcoverde, in the state of Pernambuco, Brazil. I am looking for an opportunity to start my career as a junior developer. I started my studies in programming at the end of 2021 and decided to dedicate myself to technology in April 2022, after being delighted with web development. Every day I learn something different, following tips from more experienced developers. I'm willing to learn new technologies and hone my skills.</p>
            <div>
                <a href="https://my-portfolio-dev-a4a9c.web.app/curriculo.pdf" class="link-action bg-accent" download="curriculo.pdf">Download CV</a>
            </div>
        </div>
        <div class="skills bg-accent3 flex">
            <div class="skill-single">
                <Skill title="Html 5" :level="4"/>
            </div>
            <div class="skill-single">
                <Skill title="Css 3" :level="3"/>
            </div>
             <div class="skill-single">
                <Skill title="JavaScript" :level="2"/>
            </div>
            <div class="skill-single">
                <Skill title="Vue JS" :level="3"/>
            </div>
            <div class="skill-single">
                <Skill title="Bootstrap" :level="1"/>
            </div>
            <div class="skill-single">
                <Skill title="Spectre" :level="2"/>
            </div>
            <div class="skill-single">
                <Skill title="Vuex" :level="1"/>
            </div>
            <div class="skill-single">
                <Skill title="Git" :level="1"/>
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