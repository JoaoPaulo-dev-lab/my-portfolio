<template>
  <footer class="footer flex items-center justify-center text-accent bg-secundary position-relative">
    <p>
        João Paulo Maciel &copy;<span id="year"></span>
    </p>
  </footer>
</template>

<script>
export default {
    name: "FooterApp",

    methods: {
      getFullYear() {
            const year = document.getElementById('year')
            const anoAtual = new Date();
            year.innerHTML = anoAtual.getFullYear();
        }
    },

    mounted() {
      this.getFullYear()
    }

}
</script>

<style>
.footer{
    padding: 18px 3%;
    width: 100%;
}

.footer p{
    font-size: 15px;
}

</style>