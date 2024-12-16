<template>
    <div class="w-full bg-primary p-5">
        <div class="row grid md:grid-cols-3 gap-10 mb-10 md:mb-60">
            <div>
                <h1 class="text-4xl font-medium text-white leading-none relative w-[200px] text-justify mb-5">
                    <div class="w-8 h-8 rounded-full bg-white absolute top-0 right-4"></div>
                    École<br> 
                    de joaillerie<br>
                    de Québec
                </h1>
                <h1 class="text-4xl font-medium text-white leading-none relative w-[200px] text-justify mb-5">
                    <div class="absolute top-1 right-10 space-y-[2px]">
                        <div class="w-8 h-1.5 bg-white"></div>
                        <div class="w-8 h-1.5 bg-white"></div>
                        <div class="w-8 h-1.5 bg-white"></div>
                        <div class="w-8 h-1.5 bg-white"></div>
                        <div class="w-8 h-1.5 bg-white"></div>
                    </div>
                    +1  855<br>
                    648 8003
                </h1>
                
            </div>
            <div class="w-full max-w-sm text-white text-xl md:text-3xl">
                <p class="mb-5">
                    299, 3e Avenue Québec (Québec) G1L 2V7
                </p>
                <p>
                    info@ <br>
                    ecoledejoaillerie.ca
                </p>
            </div>
            <div class="w-full max-w-sm text-white text-xl">
                <p class="mb-10">
                    Administration:<br>
                    Lundi au jeudi:  8h à 12h - 13h à 16h
                </p>
                <p>
                    Inscris-toi à notre infolettre pour recevoir en primeur la liste des nouvelles formations et ne manquer aucun événement.
                </p>
                <p class="border-b border-white py-3 text-white/50">
                    Adresse courriel
                </p>
            </div>
        </div>
        <div class="row grid grid-cols-2 md:grid-cols-3 gap-10">
            <ul class="md:flex gap-10 md:gap-5 text-white">
                <li>
                    <a href="">Facebook</a>
                </li>
                <li>
                    <a href="">Instagram</a>
                </li>
                <li>
                    <a href="">YouTube</a>
                </li>
            </ul>
            <ul class="md:flex gap-10 md:gap-5 text-white">
                <li>
                    <a href="">Politiques et confidentialités</a>
                </li>
                <li>
                    <a href="">FAQ</a>
                </li>
            </ul>
            <div class="text-white text-sm md:text-lg col-span-2 md:col-span-1">
                <p>
                    © Tous droit réserver à l’École de joaillerie de Québec  {{ year }}
                </p>
            </div>
        </div>

    </div>
</template>
<script setup>
const year = computed(()=>{
    return new Date().getFullYear();
})
</script>
<style scoped>
a{
    @apply text-white text-lg underline
}
</style>