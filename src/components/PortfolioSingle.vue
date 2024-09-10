<template>
  <div class="portfolio-single flex column" @click="openLink">
    <div class="bg" :style="{'background-image': `url('${path}')`}">
    </div>
    <div class="flex items-center">
        <i class="fa fa-circle text-accent"></i>
        <span class="text-secundary">{{title}}</span>
    </div>
  </div>
</template>

<script>

export default {
    name: 'PortfolioSingle',
    props: {
        path: String, // Caminho
        title: String,
        link: String
    },

    methods:{
        openLink(){
            window.open(this.link)
        }
    }
}
</script>

<style>
 .portfolio-single{
    width: 31%;
    height: 300px;
    margin-bottom: 30px;
    border-radius: 10px;
    transition: 0.5s;
 }

 .portfolio-single .bg{
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 100%;
    margin-bottom: 15px;
     border-radius: 10px;
     cursor: pointer;
     

 }

 .portfolio-single:hover{
     width: 32%;
 }

 .portfolio-single i{
    margin-right: 6px;
 }

@media screen and (max-width: 1000px){
    .portfolio-single{
    width: 47%;
    height: 280px;
 }

 .portfolio-single:hover{
     width: 48%;
 }
}

@media screen and (max-width: 700px) {
    .portfolio-single{
    width: 100%;
    height: 350px;
}

    .portfolio-single:hover{
     width: 100%;
 }
}


@media screen and (max-width: 450px) {
    .portfolio-single{
    width: 100%;
    height: 280px;}

    .portfolio-single:hover{
     width: 100%;
 }
}

</style>