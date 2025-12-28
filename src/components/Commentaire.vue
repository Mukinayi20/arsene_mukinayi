<template>
    <div class="pb-15 flex flex-col justify-center">
        <div class="pt-20">
            <TitleCard className="flex items-center flex-col gap-5 pb-10">
                <svg xmlns="http://www.w3.org/2000/svg" width="60" height="60" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-message-square-more-icon lucide-message-square-more"><path d="M22 17a2 2 0 0 1-2 2H6.828a2 2 0 0 0-1.414.586l-2.202 2.202A.71.71 0 0 1 2 21.286V5a2 2 0 0 1 2-2h16a2 2 0 0 1 2 2z"/><path d="M12 11h.01"/><path d="M16 11h.01"/><path d="M8 11h.01"/></svg>
                Commentaire
            </TitleCard>
        </div>
        <div class="flex justify-center items-center gap-2 pl-4">
            <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-album-icon lucide-album desktop:w-7"><rect width="18" height="18" x="3" y="3" rx="2" ry="2"/><polyline points="11 3 11 11 14 8 17 11 17 3"/></svg>
            <div class="w-210">
                <h3 class="tablette:text-2xl text-xl desktop:p-none text-Foreground">Tous les commentaires</h3>
            </div>
        </div>
        <div v-if="commentaires.length > 0" class="flex flex-col items-center">
            <div class="desktop:w-210 flex flex-col justify-center">
                <Layoutprimary v-for="commentaire in voir" :key="commentaire.id" class="hover:border-accent/50">
                    <div class="flex justify-between">
                        <h3 class="text-lg text-primary">{{ commentaire.fullname }}</h3> <div class="text-mutedForeground flex items-center text-sm">{{ formatDate(commentaire.date) }}</div>
                    </div>
                    <p class="pt-5 text-primary">"{{ commentaire.commentaire }}"</p>
                </Layoutprimary>
            </div>
            <div class="flex justify-center gap-8 flex-wrap">
                <div v-if="commentaires.length > 3">
                    <Button @click="showAll = !showAll" extra-class="flex items-center gap-3 bg-background border-secondary hover:border-[#00d3f2]/40 w-max">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#41494F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-down-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"/></svg>
                        <template #btn-primary>Voir plus</template>
                    </Button>
                </div>
                <Button extra-class="flex items-center gap-3 bg-[#00d3f2]/10 border-[#00d3f2]/40 hover:bg-[#00d3f2]/20 w-max">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#41494F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-plus-icon lucide-plus"><path d="M5 12h14"/><path d="M12 5v14"/></svg>
                    <template #btn-primary>Laisser un commentaire</template>
                </Button>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

import TitleCard from './TitleCard.vue';
import Button from './Button.vue';
import Layoutprimary from './Layoutprimary.vue';
import { formatDate, voirPlusMooin } from '@/js/config';


const commentaires = ref([
    {id: 1, fullname: 'Marie Dubois', commentaire: 'Excellent travail! J\'adore le design minimaliste et la fluidité de la navigation.', date: new Date()},
    {id: 2, fullname: 'Jean Martin', commentaire: 'Portfolio très impressionnant. Les projets sont présentés de manière très professionnelle.', date: new Date()},
    {id: 3, fullname: 'Sophie Laurent', commentaire: 'L\'animation de la photo de profil au scroll est vraiment réussie. Bravo!', date: new Date()},
    {id: 4, fullname: 'Rose Mukinayi', commentaire: 'Tu as fais du très bon travail j\'apprecie ton sens du detail. Merci !', date: new Date()},
    {id: 4, fullname: 'Elyse Mukinayi', commentaire: 'J\'apprecie beaucoup ton travail, is perfect. Merci !', date: new Date()},
])

const showAll = (false)

const voir = voirPlusMooin(commentaires, showAll)

</script>