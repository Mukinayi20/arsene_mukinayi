<template>
    <!-- <div class="primary-center hidden fixed z-1 rounded-full ml-4 opacity-50 border border-accent/75 desktop:hover:opacity-80 hover:scale-125 transition delay-150 duration-400 ease-in-out desktop:ml-70">
        <img class="w-17 h-17 rounded-full object-cover" src="/IMG-20250901-WA0029.jpg" alt="Profil">
    </div> -->
    <header id="nav-bar" class="text-Foreground lg:pb-30">
        <nav class="nav-bar border-b border-secondary fixed items-center top-0 z-2 desktop:pl-40 desktop:pr-40 desktop:font-semibold">
            <a href="#nav-bar" class="nav-bar__title dark:text-primary/90">Arsène MK</a>
            <div class="hidden desktop:flex desktop:gap-8 dark:text-primary/40">
                <a href="#apropos" class="group nav-bar__link">
                    <div class="link-anime"></div>
                    <div>À propos</div>
                </a>
                <a href="#projet" class="group nav-bar__link">
                    <div class="link-anime"></div>
                    <div>Projets</div>
                </a>
                <a href="#contact" class="group nav-bar__link">
                    <div class="link-anime"></div>
                    <div>Contact</div>
                </a>
            </div>
            <div class="flex gap-4">
                <BtnTheme />
                <a href="#contact" class="relative group p-2 text-accent font-medium border border-accent/30 rounded-xl pl-4 pr-4 transition-transform duration-500 hover:scale-105 origin-left ease-in-out">
                    <div class="absolute inset-0 w-0 bg-accent/10 rounded-xl transition-all duration-500 ease-in-out group-hover:w-full"></div>
                    <div class="relative z-10">Me contacter</div>
                </a>
            </div>
        </nav>
        <div class="flex justify-center">
            <div class="w-[70%] flex flex-col lg:flex-row items-center justify-between mt-[200px]">
                <div class="primary-center" ref="bigImage">
                    <img class="h-120 object-cover border-2 border-accent/50 rounded-2xl" src="/IMG-20250901-WA0029.jpg" alt="Profil" />
                    <!-- header-profil transition-transfordesktop:w200m duration-20 ease-in-out shadow-[0px_0px_50px_-15px_#4D9FA3]" :style="{ transform: `scale(${scale})` } "effer pendant le scrole du profil" -->
                </div>
                <div class="sm:max-md:pt-100">
                    <div class="flex justify-center items-center primary-center mt-7 h-5 gap-4">
                        <h1 class="tablette:text-[3.4rem] max-sm:text-3xl text-[2.3rem] text-primary transition duration-500 hover:animate-leaf ease-in-out dark:text-primary/80">Arsène Mukinayi</h1>
                        <div class="group border border-accent rounded-full p-2 transition duration-400 hover:scale-110 ease-in-out cursor-pointer animate-leaf">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-badge-info-icon lucide-badge-info transition duration-400 group-hover:rotate-15">
                                <path d="M3.85 8.62a4 4 0 0 1 4.78-4.77 4 4 0 0 1 6.74 0 4 4 0 0 1 4.78 4.78 4 4 0 0 1 0 6.74 4 4 0 0 1-4.77 4.78 4 4 0 0 1-6.75 0 4 4 0 0 1-4.78-4.77 4 4 0 0 1 0-6.76Z" />
                                <line x1="12" x2="12" y1="16" y2="12" />
                                <line x1="12" x2="12.01" y1="8" y2="8" />
                            </svg>
                        </div>
                    </div>
                    <div class="primary-center h-70 p-8">
                        <p class="text-center lg:text-end text-lg text-mutedForeground desktop:w-180">Je conçois des produits numériques qui transforment des idées complexes en expériences simples, utiles et accessibles.</p>
                    </div>
                </div>
                <!-- <div class="flex gap-4 justify-center">
                    <Button extraClass="text-primaryForeground transition duration-400 hover:scale-103 bg-accent ease-in-out">
                        <template #btn-primary>Voir mes projets</template>
                    </Button>
                    <Button extraClass="border-secondary dark:border-accent/20 transition transition duration-400 hover:scale-103 ease-in-out overflow-hidden after:content-[''] after:absolute after:inset-0 after:bg-accent/10 after:rounded-xl after:scale-x-0 after:origin-left after:transition-transform after:duration-500 after:ease-in-out hover:after:scale-x-100 dark:text-primary/80">
                        <template #btn-primary>Me contacter</template>
                    </Button>
                </div> -->
            </div>
        </div>
        <a href="#apropos" class="hidden lg:flex justify-center pt-25">
            <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" fill="none" stroke="#41494F" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-down-icon lucide-chevron-down animate-bounce"><path d="m6 9 6 6 6-6" /></svg>
        </a>
    </header>
</template>

<script setup>
import { onMounted, onUnmounted, ref } from "vue";
import Button from "./Button.vue";
import BtnTheme from "./btn/BtnTheme.vue";

// const scale = ref(1);

// const handelScroll = () => {
//     const scrollY = window.scrollY;

//     const newScale = 1 - scrollY / 400;
//     scale.value = Math.max(newScale, 0.3);
// };

// onMounted(() => {
//     window.addEventListener("scroll", handelScroll);
// });

// onUnmounted(() => {
//     window.addEventListener("scroll", handelScroll);
// });
</script>
