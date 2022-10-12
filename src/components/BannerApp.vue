<template>
  <section class="banner flex justify-around nowrap items-center" id="home">
    <div class="flex justify-center  column">
        <div>
            <p class="text-secundary">Olá, meu nome é</p>
        </div>
        <div>
            <h1 class="text-bolder text-primary">João Paulo Maciel</h1>
        </div>
        <div class="flex nowrap items-center">
            <div class="row-accent"></div>
            <p class="text-secundary">Desenvolvedor Front-end</p>
        </div>
        <div class="link-action-position">
            <a href="https://github.com/JoaoPaulo-dev-lab" class="link-action bg-accent text-bold">Meu GitHub</a>
        </div>
    </div>
    <div class="avatar-container">
        <div class="border-accent">
            <img src="../assets/images/img2.jpg" alt="">
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'BannerApp'
}
</script>

<style>
    .banner{
        width: 100%;
        height: 500px;
        padding: 0 3%;
        /* Created with https://www.css-gradient.com */
        background: #010101;
        background: -webkit-linear-gradient(left, #010101, #1B1B1B);
        background: -moz-linear-gradient(left, #010101, #1B1B1B);
        background: linear-gradient(to right, #010101, #1B1B1B);
    }

    .banner h1{
        font-size: 60px;
        margin: 10px 0;
    }

    .banner p{
        font-size: 14px;
    }

    .avatar-container .border-accent{
        border: 15px solid #edb45f57;
        width: 350px;
        height: 350px;
        border-radius: 175px;
    }

    .avatar-container .border-accent img{
        width: 100%;
        height: 100%;
        border-radius: 50%;
        border: 8px solid rgba(0, 0, 0, 0);
    }

    @media screen and (max-width: 940px) {
        .banner{
        height: auto;
        padding: 50px 3%;
        }

        .avatar-container{
            display: none;
        }

        .link-action-position{
            width: 100%;
            text-align: center;
        }

        
    }

    @media screen and (max-width: 610px) {
        .banner h1{
        font-size: 40px;
       }
    }

    @media screen and (max-width: 405px) {
        .banner h1{
        font-size: 30px;
    }
    }
</style>