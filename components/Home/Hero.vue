<template>
    <div class="w-full h-[100vh] bgImage flex flex-col items-center justify-between gap-5">
        <div class="row">
            <HomeNavigation/>
            <div class="w-full h-full overflow-hidden flex flex-col items-center">
                <img src="/images/white-dots.png" class="h-max min-w-max"/>
            </div>
            <div class="p-5 absolute bottom-0">
                <p class="text-white text-3xl" style="text-shadow: 0 0 3px #000;">
                    Matérialise 
                    <br>ta créativité 
                </p>
            </div>
        </div>
        
    </div>
</template>
<style scoped>
.bgImage{
    background-image: url('/images/hero.png');
    @apply bg-top bg-no-repeat bg-cover
}

</style>