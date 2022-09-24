<template>
    <header class="header flex items-center justify-between bg-primary">
        <div class="flex items-center">
            <div class="header-avatar bg-accent3"></div>
            <span class="title-section text-accent">João Paulo</span>
        </div>
        <div class="menu-desktop">
           <nav>
            <ul class="flex items-center">
                <li>
                    <a class="text-primary" href="">Home</a>
                </li>
                <li>
                    <a class="text-primary" href="">About</a>
                </li>
                <li>
                    <a class="text-primary" href="">Services</a>
                </li>
                <li>
                    <a class="text-primary" href="">Portfólio</a>
                </li>
                <li>
                    <a class="text-primary" href="">Contato</a>
                </li>
            </ul>
           </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderApp'
}
</script>

<style>
.header{
    width: 100%;
    padding: 10px 3%;

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
.menu-desktop ul li a{
    font-size: 13px;
}

.menu-desktop ul li a:hover{
    color: #edb45f;
}

</style>