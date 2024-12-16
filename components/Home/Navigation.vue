<template>
    <div class="w-full flex justify-between gap-5 p-5  py-3">
        <div>
            <h1 class="text-lg font-medium text-white leading-none">
                École<br> 
                de joaillerie<br>
                de Québec
            </h1>
        </div>
        <!-- Desktop Nav -->
        <div class="text-white hidden md:grid md:grid-cols-4 gap-10">
            <ul>
                <li class="inscription">
                    <div class="dot"></div>
                    <NuxtLink to="">
                        Inscription
                    </NuxtLink>
                    <ul class="sub-menu">
                        <li>
                            <NuxtLink to="">
                                Cours de loisirs
                            </NuxtLink>
                        </li>
                        <li>
                            <NuxtLink to="">
                                Ateliers
                            </NuxtLink>
                        </li>
                        <li>
                            <NuxtLink to="">
                                DEC
                            </NuxtLink>
                        </li>
                    </ul>
                </li>
            </ul>
            <ul>
                <li>
                    <NuxtLink to="">
                        À propos
                    </NuxtLink>
                </li>
            </ul>
            <ul>
                <li>
                    <NuxtLink to="">
                        Recherche
                    </NuxtLink>
                </li>
            </ul>
            <ul>
                <li>
                    <NuxtLink to="">
                        Contact
                    </NuxtLink>
                </li>
            </ul>
        </div>
        
        <!-- Mobile Nav -->
        <div class="md:hidden w-full h-screen fixed left-0 top-0 z-50 bg-primary p-5 flex flex-col justify-between" v-if="show">
            <div>
                <div class="w-full flex justify-between mb-10">
                    <h1 class="text-lg font-medium text-white leading-none">
                        École<br> 
                        de joaillerie<br>
                        de Québec
                    </h1>
                    <img src="/images/menu.png" alt="menu" class="h-6" @click="show=false">
                </div>
                <ul class="text-white text-2xl space-y-5">
                    <li>
                        <NuxtLink to="">Inscription</NuxtLink>
                        
                        <ul class="ml-14 space-y-3">
                            <li>
                                <NuxtLink to="">Cours de loisirs</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="">Ateliers</NuxtLink>
                            </li>
                            <li>
                                <NuxtLink to="">DEC</NuxtLink>
                            </li>
                        </ul>
                    </li>
                    <li>
                        <NuxtLink to="">À propos</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="">Recherche</NuxtLink>
                    </li>
                </ul>
            </div>
            <div class="w-full">
                <div class="w-full grid grid-cols-2 gap-5 mb-5">
                    <ul>
                        <li>
                            <a href="" class="link">Facebook</a>
                        </li>
                        <li>
                            <a href="" class="link">Instagram</a>
                        </li>
                        <li>
                            <a href="" class="link">YouTube</a>
                        </li>
                    </ul>
                    <a href="" class="link">Politiques et confidentialités</a>
                </div>
                <div class="text-white text-lg">
                    <p>
                        © Tous droit réserver à l’École de joaillerie de Québec  {{ year }}
                    </p>
                </div>
            </div>
        </div>
        <div class="md:hidden">
            <img src="/images/menu.png" alt="menu" class="h-6" @click="show=true">
        </div>
    </div>
</template>
<script setup>
const show = ref(true)
const year = computed(()=>{
    return new Date().getFullYear();
})
</script>
<style scoped>
.link{
    @apply text-white text-lg underline
}
li{
    @apply cursor-pointer
}
.dot{
    @apply w-1 h-1 rounded-full bg-white absolute top-0 right-0 hidden;
}
.inscription{
    @apply relative
}
.sub-menu{
    @apply absolute top-6 w-max grid-cols-3 gap-10 hidden;
}
.inscription:hover .sub-menu{
    @apply grid
}
.inscription:hover .dot{
    @apply block
}
</style>