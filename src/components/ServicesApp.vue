<template>
  <section class="services-app bg-accent3">
    <SectionTitle title="My Services" subtitle="What Can I Do"/>
    <div class="container-services flex wrap justify-between">
        <ServiceSingle title="Creative Design" icon="fa fa-pencil" description="Lorem Ipsum é simplesmente uma simulação de texto da indústria tipográfica e de impressos, e"/>
        <ServiceSingle title="Branding" icon="fa fa-flag" description="Lorem Ipsum é simplesmente uma simulação de texto da indústria tipográfica e de impressos, e"/>
        <ServiceSingle title="User Interface" icon="fa fa-tablet" description="Lorem Ipsum é simplesmente uma simulação de texto da indústria tipográfica e de impressos, e"/>
        <ServiceSingle title="Creative Design" icon="fa fa-code" description="Lorem Ipsum é simplesmente uma simulação de texto da indústria tipográfica e de impressos, e"/>
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