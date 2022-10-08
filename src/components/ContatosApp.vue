<template>
  <div class="footer-app bg-secundary flex items-center justify-center">
    <a class="bg-primary text-primary flex items-center justify-center" href="">
        <i class="fab fa-whatsapp"></i>
    </a>
    <a class="bg-primary text-primary flex items-center justify-center" href="">
        <i class="fab fa-instagram"></i>
    </a>
    <a class="bg-primary text-primary flex items-center justify-center" href="">
        <i class="fab fa-linkedin"></i>
    </a>
    <a class="bg-primary text-primary flex items-center justify-center" href="">
        <i class="fa fa-envelope"></i>
    </a>
  </div>
</template>

<script>
export default {
    name: 'ContatosApp'
}
</script>

<style>
    .footer-app{
        padding: 15px 3%;
    }

    .footer-app a{
        width: 40px;
        height: 40px;
        border-radius: 20px;
        text-decoration: none;
        font-size: 19px;
        margin: 0 15px;
    }
    
</style>