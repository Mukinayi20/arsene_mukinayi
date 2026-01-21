<template>
    <div class="border-t border-secondary p-8 flex justify-center">
        <div class="flex flex-col items-center tablette:w-200">
            <section class="flex flex-wrap items-top gap-15 pb-8 tablette:w-full tablette:justify-between justify-around">
                <div class="flex flex-col text-Foreground/80">
                    <div class="flex items-Center pb-3">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-dot-icon lucide-dot"><circle cx="12.1" cy="12.1" r="1"/></svg>
                        <h3 class="text-lg text-primary">Sections</h3>
                    </div>
                    <div class="flex flex-col ml-6 gap-2 dark:text-primary">
                        <a href="#apropos" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">À propos</a>
                        <a href="#projet" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">Projets</a>
                        <a href="#contact" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">Contact</a>
                    </div>
                </div>
                <div class="flex flex-col text-Foreground/80">
                    <div class="flex items-Center pb-3">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-dot-icon lucide-dot"><circle cx="12.1" cy="12.1" r="1"/></svg>
                        <h3 class="text-lg text-primary">Pages</h3>
                    </div>
                    <div class="flex flex-col ml-6 gap-2 dark:text-primary">
                        <a href="#" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">Tous les projet</a>
                        <a href="/CV_Arsène_Mukinayi.pdf" class="group p-2 pl-3 pr-3 bg-secondary rounded-lg flex justify-center items-center gap-3 transition duration-400 hover:scale-105 hover:bg-accent/30 ease-in-out">Voir le cv</a>
                    </div>
                </div>
                <div>
                    <div class="flex items-Center pb-3">
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-dot-icon lucide-dot"><circle cx="12.1" cy="12.1" r="1"/></svg>
                        <h3 class="text-lg text-primary">Contact</h3>
                    </div>
                    <ReseauxSociaux/>
                </div>
            </section>
            <section class="flex border-t border-secondary pt-5 w-full">
                <small class="text-Foreground/70 dark:text-primary"> &#169; 2025 Arsène Mukinayi. Tous droits réservé. <br>Fabled Print.</small>
                <div>
    
                </div>
            </section>
        </div>
    </div>
</template>

<script setup>
import ReseauxSociaux from './collaboration/ReseauxSociaux.vue';
</script>