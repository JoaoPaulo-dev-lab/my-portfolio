<template>
    <header class="header flex items-center justify-between bg-primary position-relative">
        <div class="flex items-center">
            <img class="header-avatar bg-accent3" src="../assets/images/img2.jpg">
            <span class="my-name text-accent text-bolder">João Paulo</span>
        </div>
        <div class="menu-desktop">
           <nav>
            <ul class="flex items-center">
                <!-- <li>
                    <a class="text-primary" href="#home">Home</a>
                </li> -->
                <li>
                    <a class="text-primary" href="#about">Sobre</a>
                </li>
                <li>
                    <a class="text-primary" href="#services">Serviços</a>
                </li>
                <li>
                    <a class="text-primary" href="#portfolio">Portfólio</a>
                </li>
                
            </ul>
           </nav>
        </div>
        <div class="menu-icon">
                <i class="fa fa-bars text-primary cursor-pointer" @click="toggleMenu"></i>
        </div>
        <div class="menu-mobile position-absolute">
            
           <nav class="bg-secundary">
            <ul class="flex  column" id="menu-mobile-ul">
                <!-- <li>
                    <a class="text-primary flex justify-center" href="#home">Home</a>
                </li> -->
                <li>
                    <a class="text-primary flex justify-center" href="#about">Sobre</a>
                </li>
                <li>
                    <a class="text-primary flex justify-center" href="#services">Serviços</a>
                </li>
                <li>
                    <a class="text-primary flex justify-center" href="#portfolio">Portfólio</a>
                </li>
            </ul>
           </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderApp',
    data(){
        return {
            isVisibleMenu: false
        }
    },
    methods: {
        toggleMenu(){
            const menuElement = document.getElementById('menu-mobile-ul')
            const countChildren = menuElement.children.length
            if(this.isVisibleMenu){
                 menuElement.style.height = '0px'
                 menuElement.style.padding = '0px'
                for(let i = 0; i < countChildren; i++){
                    menuElement.children[i].style.display = 'none'
                    
                    
                }

            }
            else{
                 menuElement.style.height = '130px'
                menuElement.style.padding = '5px'
                for(let i = 0; i < countChildren; i++){
                     setTimeout(function(){
                     menuElement.children[i].style.display = 'flex'
                     clearTimeout(this)
                   }, 270)
                    
                }
            }
            this.isVisibleMenu = !this.isVisibleMenu
        }
    }
}
</script>

<style>
.header{
    width: 100%;
    padding: 10px 3%;
}

.header .my-name{
    font-size: 12px;
}

.header-avatar{
    width: 36px;
    height: 36px;
    border-radius: 18px;
    margin-right: 5px;
}
.menu-desktop ul li{
    list-style: none;
    margin-left: 20px;
}
.menu-desktop ul li a, .menu-mobile ul li a{
    font-size: 13px;
}

.menu-desktop ul li a:hover{
    color: #edb45f;
}

header .menu-mobile{
    display: none;
}

.menu-mobile nav{
    width: 100%;
}

.menu-mobile ul li{
    list-style: none;
}

.menu-icon{
    font-size: 25px;
    display: none;
}

.menu-mobile{
    width: 100%;
    top: 57px;
    left: 0;
    z-index: 9999;
}

.menu-mobile ul li a:hover{
    color: #edb45f;
}

.menu-mobile ul {
    width: 100%;
    padding: 0px;
    height: 0px;
    transition: 0.5s;
}

.menu-mobile ul li{
    display: none;
}
.menu-mobile ul li a {
    padding: 10px;
    width: 100%;
    
}

@media screen and (max-width: 700px) {
    .menu-icon{
        display: block;
    }
    header .menu-desktop{
        display: none;
    }
    header .menu-mobile{
    display: flex;
}
}

@media screen and (max-width: 450px) {
    .header .my-name{
        display: none;
    }
}

</style>