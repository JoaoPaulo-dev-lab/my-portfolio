<template>
  <section class="services-app bg-accent3">
    <SectionTitle title="Meus Serviços" subtitle="O que eu posso fazer?" idNav="services"/>
    <div class="container-services flex wrap justify-between">
        <ServiceSingle title="Design Criativo" icon="fa fa-pencil" description="Design criativo que combina com o conteúdo da Página Web"/>
        <ServiceSingle title="Interface do Usuário" icon="fa fa-tablet" description="Interface moderna com design criativo e responsivo"/>
        <ServiceSingle title="Código Limpo" icon="fa fa-code" description="Código limpo e de fácil entendimento, o que facilita manutenção futura."/>
    </div>
  </section>
</template>

<script>
import SectionTitle from './SectionTitle.vue'
import ServiceSingle from './ServiceSingle.vue'
export default {
   name: 'ServicesApp',
   components: {SectionTitle, ServiceSingle}
}
</script>

<style>
 .services-app{
    width: 100%;
    padding: 30px 3% 50px 3%;
    
 }

 .container-services{
    margin-top: 30px;
 }
</style>