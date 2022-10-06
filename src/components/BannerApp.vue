<template>
  <section class="banner flex justify-around nowrap items-center">
    <div class="flex justify-center  column">
        <div>
            <p class="text-secundary">Hello, My name is</p>
        </div>
        <div>
            <h1 class="text-bolder text-primary">João Paulo Maciel</h1>
        </div>
        <div class="flex nowrap items-center">
            <div class="row-accent"></div>
            <p class="text-secundary">Front-end Developer</p>
        </div>
        <div>
            <a href="" class="link-action bg-accent">Know More</a>
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
</style>