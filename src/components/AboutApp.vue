<template>
  <section class="bg-accent2 about">
    <SectionTitle title="About Me" subtitle="Who am I"/>
    <div class="about-box flex justify-between">
        <div class="description flex column">
            <p class="text-description text-secundary">Lorem Ipsum é simplesmente uma simulação de texto da indústria tipográfica e de impressos, e vem sendo utilizado desde o século XVI, quando um impressor desconhecido pegou uma bandeja de tipos e os embaralhou para fazer um livro de modelos de tipos. Lorem Ipsum sobreviveu não só a cinco séculos, como também ao salto para a editoração eletrônica, permanecendo essencialmente inalterado.</p>
            <div>
                <a href="" class="link-action bg-accent">Download CV</a>
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
        padding: 30px 3%;
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
</style>