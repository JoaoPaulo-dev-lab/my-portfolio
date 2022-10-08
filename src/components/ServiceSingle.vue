<template>
  <div class="service-single bg-accent2 flex column items-center">
    <div>
        <i :class="icon" class="text-accent"></i>
    </div>
    <div>
        <span class="title text-primary text-bold">{{title}}</span>
    </div>
    <div>
        <p class="text-secundary description">{{description}}</p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'ServiceSingle',
    props: {
        icon: String,
        title: String,
        description: String
    }
}
</script>

<style>
    .service-single{
        width: 32%;
        padding: 20px 10px;
        margin-bottom: 20px;
    }

    .service-single i{
        font-size: 30px;
        margin-bottom: 10px;
    }

    .service-single .title{
        font-size: 14px;
    }

    .service-single .description{
        font-size: 11px;
        text-align: center;
        margin-top: 7px;
    }

    @media screen and (max-width: 550px){
        .service-single{
        width: 48%;
     }
    }
</style>