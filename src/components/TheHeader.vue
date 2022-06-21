<template>
    <div class="container">
        <img src="/img/la-molisana-logo.png" alt="">

        <ul class="nav justify-content-center">
            <li class="nav-item" v-for="(link, i) in navLinks" :key="i">
                <a class="nav-link" aria-current="page" :href="link.href">{{link.name}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "TheHeader",
    data(){
        return{
            navLinks: [
                {
                    name: "Home",
                    href: "#",
                },
                {
                    name: "Prodotti",
                    href: "#",
                },
                {
                    name: "Chi Siamo",
                    href: "#",
                },
                {
                    name: "Contatti",
                    href: "#",
                },
                ]
        }
    }
}
</script>

<style>

</style>