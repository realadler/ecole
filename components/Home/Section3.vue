<template>
    <div class="w-full  bg-white md:p-5">
        <div class="row bgImage p-5 md:p-0">
            <p class="text-black max-w-3xl text-3xl xl:text-5xl mb-60 md:mb-10">
                L’École de joaillerie de Québec, fondée par deux artisans pour assurer l’avenir du bijou québécois, est un lieu où créativité et savoir-faire se rencontrent pour former les joailliers de demain. 
                <br><br>
                À l’aube de ses 40 ans, l’EJQ demeure fidèle à sa mission de transmission et, avec une vision novatrice, attire ceux qui rêvent de créer des bijoux de leurs propres mains. 
            </p>
            <a href="" class="text-lg underline font-medium">
                En savoir plus
            </a>

        </div>


    </div>
    
</template>
<style scoped>
.bgImage{
    background-size: 600px;
    background-image: url('/images/blue-dot.png');
    @apply bg-right bg-no-repeat bg-contain
}
@media screen and (max-width:768px) {
    .bgImage{
        background-size: 280px;
        background-image: url('/images/blue-mob.png');
        background-position-x: right;
        background-position-y: bottom;  
        @apply bg-no-repeat
    }
}
</style>