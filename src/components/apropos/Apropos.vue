<template>
<div id="apropos" class="flex flex-col justify-center items-center">
    <div class="flex items-center flex-col gap-4 mt-20 p-8">
        <div>
            <TitleCard className="flex items-center flex-col gap-4 dark:text-primary/80">À propos</TitleCard>
        </div>
        <p class="text-center text-lg text-mutedForeground pt-15 desktop:w-180">Je développe des solutions numériques full stack à partir de besoins concrets. De l’analyse à la mise en production, je conçois des interfaces fluides et performantes, pensées pour simplifier les usages, automatiser les processus et faire gagner du temps, tout en créant une réelle valeur business</p>
    </div>
        <Layoutprimary class="mt-15 desktop:w-200 transition duration-700 hover:-translate-y-1 ease-in-out hover:shadow-[0px_10px_93px_-73px_#4D9FA3]">
            <div class="flex flex-col justify-between">
                <div class="flex justify-between items-center">
                    <h2 class="text-primary text-2xl font-medium">Résumé</h2>
                    <div class="flex gap-4">
                        <a href="/CV_Arsène_Mukinayi.pdf" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke=currentColor stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-eye-icon lucide-eye text-primary transition duration-400"><path d="M2.062 12.348a1 1 0 0 1 0-.696 10.75 10.75 0 0 1 19.876 0 1 1 0 0 1 0 .696 10.75 10.75 0 0 1-19.876 0"/><circle cx="12" cy="12" r="3"/></svg>
                            <span class="hidden tablette:block text-primary font-semibold">Voir le cv</span>
                        </a>
                        <a href="/CV_Arsène_Mukinayi.pdf" download="/CV_Arsène_Mukinayi.pdf" class="p-2 pl-3 pr-3 gap-3 bg-secondary rounded-lg flex justify-center items-center transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke=currentColor stroke-width="3" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-download-icon lucide-download text-primary"><path d="M12 15V3"/><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><path d="m7 10 5 5 5-5"/></svg>
                            <span class="hidden tablette:block text-primary font-semibold">Télécharger</span>
                        </a>
                    </div>
                </div>
                <div>
                    <p class="text-lg text-mutedForeground pt-10">"Développeur Full Stack et architecte de solutions web, je me spécialise dans la conception d'interfaces modernes et d'architectures numériques robustes. Fort d'une expertise technique centrée sur TypeScript, Node.js et l'écosystème JavaScript (AdonisJS), je m'attache à transformer des concepts complexes en applications fluides, alliant une rigueur backend pointue à une élégance frontend soignée."</p>
                    <div class="flex items-Center pt-5">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-dot-icon lucide-dot"><circle cx="12.1" cy="12.1" r="1"/></svg>
                        <h3 class="text-lg text-primary">compétences techniques</h3>
                    </div>
                </div>
            </div>
            <div class="flex flex-wrap gap-2 pt-5 pb-2">
                <Cardtech/>
            </div>
            <div class="flex items-Center pt-5">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-dot-icon lucide-dot"><circle cx="12.1" cy="12.1" r="1"/></svg>
                <h3 class="text-lg text-primary">Savoir être</h3>
            </div>
            <div class="flex flex-wrap gap-2 pt-5 pb-2">
                <compTech/>
            </div>
        </Layoutprimary>
        <div class="mt-20 mb-25 w-full tablette:flex tablette:flex-wrap tablette:justify-center z-1">
            <Layoutprimary auther-class="group hover:border-accent/30 tablette:w-80 transition-transform duration-800 delay-300 hover:scale-110 transition-colors hover:bg-gradient-to-r hover:from-[#d8e7e7] hover:to-[#dae9e9] transition-shadow hover:shadow-[0_20px_60px_-20px_rgba(77,159,163,0.20)] ease-in-out" class="dark:transition dark:duration-800 dark:hover:border-accent dark:hover:from-accent/5  dark:hover:via-accent/10 dark:hover:to-accent/6">
                <div class="bg-secondary/50 w-max p-3 rounded-lg group-hover:bg-accent/40 transition duration-700 group-hover:rotate-20 group-hover:shadow-[0_26px_100px_-10px_#fff] dark:group-hover:shadow-none ease-in-out">
                    <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-code-xml-icon lucide-code-xml"><path d="m18 16 4-4-4-4"/><path d="m6 8-4 4 4 4"/><path d="m14.5 4-5 16"/></svg>
                </div>
                <ContentCard classTitle="transition duration-700 group-hover:text-accent ease-in-out">
                    <template #head>Développement</template>
                    <template #main>Vue.js, Adonis.js, Typescript, Node.js</template>
                </ContentCard>
            </Layoutprimary>
            <Layoutprimary auther-class="group hover:border-accent/30 tablette:w-80 transition-transform duration-800 delay-300 hover:scale-110 transition-colors hover:bg-gradient-to-r hover:from-[#d8e7e7] hover:to-[#dae9e9] transition-shadow hover:shadow-[0_20px_60px_-20px_rgba(77,159,163,0.20)] ease-in-out" class="dark:transition dark:duration-800 dark:hover:from-accent/5 dark:hover:border-accent dark:hover:via-accent/10 dark:hover:to-accent/6">
                <div class="bg-secondary/50 w-max p-3 rounded-lg group-hover:bg-accent/40 transition duration-700 group-hover:rotate-20 group-hover:shadow-[0_26px_100px_-10px_#fff] dark:group-hover:shadow-none ease-in-out" >
                    <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-palette-icon lucide-palette"><path d="M12 22a1 1 0 0 1 0-20 10 9 0 0 1 10 9 5 5 0 0 1-5 5h-2.25a1.75 1.75 0 0 0-1.4 2.8l.3.4a1.75 1.75 0 0 1-1.4 2.8z"/><circle cx="13.5" cy="6.5" r=".5" fill="currentColor"/><circle cx="17.5" cy="10.5" r=".5" fill="currentColor"/><circle cx="6.5" cy="12.5" r=".5" fill="currentColor"/><circle cx="8.5" cy="7.5" r=".5" fill="currentColor"/></svg>
                </div>
                <ContentCard classTitle="transition duration-700 group-hover:text-accent ease-in-out">
                    <template #head>Design</template>
                    <template #main>UI/UX, Design Systems</template>
                </ContentCard>
            </Layoutprimary>
            <Layoutprimary auther-class="group hover:border-accent/30 tablette:w-80 transition-transform duration-800 delay-300 hover:scale-110 transition-colors hover:bg-gradient-to-r hover:from-[#d8e7e7] hover:to-[#dae9e9] transition-shadow hover:shadow-[0_20px_60px_-20px_rgba(77,159,163,0.20)] ease-in-out" class="dark:transition dark:duration-800 dark:hover:from-accent/5 dark:hover:border-accent dark:hover:via-accent/10 dark:hover:to-accent/6">
                <div class="bg-secondary/50 w-max p-3 rounded-lg group-hover:bg-accent/40 transition duration-700 group-hover:rotate-20 group-hover:shadow-[0_26px_100px_-10px_#fff] dark:group-hover:shadow-none ease-in-out">
                    <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-zap-icon lucide-zap"><path d="M4 14a1 1 0 0 1-.78-1.63l9.9-10.2a.5.5 0 0 1 .86.46l-1.92 6.02A1 1 0 0 0 13 10h7a1 1 0 0 1 .78 1.63l-9.9 10.2a.5.5 0 0 1-.86-.46l1.92-6.02A1 1 0 0 0 11 14z"/></svg>
                </div>
                <ContentCard classTitle="transition duration-700 group-hover:text-accent ease-in-out">
                    <template #head>Performance</template>
                    <template #main>Performance & Accessibilité</template>
                </ContentCard>
            </Layoutprimary>
        </div>
</div>
</template>

<script setup>
import Cardtech from './Cardtech.vue';
import Layoutprimary from '../Layoutprimary.vue';
import ContentCard from '../ContentCard.vue';
import TitleCard from '../TitleCard.vue';
import compTech from './compTech.vue';
</script>