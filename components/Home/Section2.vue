<template>
    <div class="w-full bg-primary text-white p-5">
        <div class="row">
            <h2 class="text-4xl font-medium mb-5">
                Nos programmes
            </h2>
            <div class="w-full grid md:grid-cols-3 gap-10">
                <div class="grid-item" v-for="el in cards" :key="el">
                    <div class="texts">
                        <h3>
                            {{ el.title }}
                        </h3>
                        <p>
                            {{ el.text }}
                        </p>
                    </div>
                    <a :href="el.link" class="underline text-lg">
                        {{ el.linkLabel }}
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
const cards = ref([
    { 
        title:'Diplôme d’études collégiales (DEC)',
        text:'Le DEC en Techniques de métiers d’art- option joaillerie, est offert par le Cégep Limoilou et s’échelonne sur trois ans. Vous y développerez votre sens artistique, vos compétences techniques ainsi que des aptitudes en gestion, vous permettant d’être autonome et de lancer votre propre entreprise.',
        linkLabel:'Inscription ↗',
        link:''
    },
    { 
        title:'Cours de loisirs ',
        text:'Les cours de loisirs offrent l’occasion d’acquérir de nouvelles habiletés créatives et de décrocher de votre quotidien. Chaque session de 12 semaines vous permet d’apprendre à votre rythme, sans évaluation, tout en repartant avec les bijoux que vous réalisez. Vous pratiquerez des exercices pour maîtriser les gestes de base et laisser libre cours à votre créativité.',
        linkLabel:'Inscription',
        link:''
    },
    { 
        title:'Ateliers de perfectionnement',
        text:'Ces ateliers s’adressent à la communauté joaillière et aux métiers d’art. Ces blocs d’apprentissage permettent d’affiner les compétences techniques et artistiques des artisans, généralement sur une à trois journées. Des formations, telles que la coulée à la cire perdue ou l’enfilage de colliers de perles, sont offertes, pour n’en nommer que quelques-unes.',
        linkLabel:'Inscription',
        link:''
    },
])
</script>
<style scoped>
.grid-item{
    @apply h-max max-w-sm flex flex-col justify-between md:space-y-20
}
.grid-item h3{
    @apply text-2xl mb-5
}
.grid-item .texts{
    @apply md:h-[400px] mb-5
}
</style>