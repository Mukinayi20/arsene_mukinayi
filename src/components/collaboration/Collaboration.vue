<template>
    <div id="contact" class="pt-20">
        <TitleCard className="flex items-center flex-col gap-5 pb-6 dark:text-primary/80"> Travaillons ensemble </TitleCard>
    </div>
    <div class="p-8 flex flex-col items-center">
        <p class="text-center text-lg text-mutedForeground desktop:w-210">Ouvert à de nouveaux projets et collaborations, je suis disponible pour échanger et étudier ensemble des solutions adaptées à vos besoins.</p>
    </div>
    <div class="flex flex-wrap justify-center gap-4 pt-5 pb-15">
        <a href="mailto:arsenemukinayi20@gmail.com" target="_blank" alt="me faire un mail" class="z-1">
            <Button extraClass="border-secondary transition transition duration-400 hover:scale-103 ease-in-out overflow-hidden after:content-['']   after:absolute after:inset-0 after:bg-accent/10 after:rounded-xl after:scale-x-0 after:origin-left after:transition-transform after:duration-500 after:ease-in-out hover:after:scale-x-100 flex gap-5 items-center text-primary dark:text-primary/90 dark:border-accent/50">
                <template #btn-primary
                    >Me faire un mail
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mails-icon lucide-mails">
                        <path d="M17 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2v-8a2 2 0 0 1 1-1.732" />
                        <path d="m22 5.5-6.419 4.179a2 2 0 0 1-2.162 0L7 5.5" />
                        <rect x="7" y="3" width="15" height="12" rx="2" /></svg
                ></template>
            </Button>
        </a>
        <a href="tel:+243821600256" class="z-1">
            <Button extraClass="border-secondary transition transition duration-400 hover:scale-103 ease-in-out overflow-hidden after:content-['']   after:absolute after:inset-0 after:bg-accent/10 after:rounded-xl after:scale-x-0 after:origin-left after:transition-transform after:duration-500 after:ease-in-out hover:after:scale-x-100 flex gap-3 items-center dark:text-primary/90 text-primary dark:border-accent/50">
                <template #btn-primary
                    >M'appeler
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4D9FA3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-phone-outgoing-icon lucide-phone-outgoing">
                        <path d="m16 8 6-6" />
                        <path d="M22 8V2h-6" />
                        <path d="M13.832 16.568a1 1 0 0 0 1.213-.303l.355-.465A2 2 0 0 1 17 15h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2A18 18 0 0 1 2 4a2 2 0 0 1 2-2h3a2 2 0 0 1 2 2v3a2 2 0 0 1-.8 1.6l-.468.351a1 1 0 0 0-.292 1.233 14 14 0 0 0 6.392 6.384" /></svg
                ></template>
            </Button>
        </a>
        <a href="wa.me/243821600256?text=Bonjour%je%suis%Arsène%Mukinayi,%que%pui-je%faire%pour%vous?">
            <Button extraClass="border-secondary transition transition duration-400 hover:scale-103 ease-in-out overflow-hidden after:content-['']   after:absolute after:inset-0 after:bg-accent/10 after:rounded-xl after:scale-x-0 after:origin-left after:transition-transform after:duration-500 after:ease-in-out hover:after:scale-x-100 flex gap-3 items-center text-accent/80 dark:border-accent/50">
                <template #btn-primary
                    >Message WhatsApp
                    <svg xmlns="http://www.w3.org/2000/svg" width="23" height="23" viewBox="0 0 16 16">
                        <path fill="#4D9FA3" d="M11.42 9.49c-.19-.09-1.1-.54-1.27-.61s-.29-.09-.42.1s-.48.6-.59.73s-.21.14-.4 0a5.13 5.13 0 0 1-1.49-.92a5.25 5.25 0 0 1-1-1.29c-.11-.18 0-.28.08-.38s.18-.21.28-.32a1.39 1.39 0 0 0 .18-.31a.38.38 0 0 0 0-.33c0-.09-.42-1-.58-1.37s-.3-.32-.41-.32h-.4a.72.72 0 0 0-.5.23a2.1 2.1 0 0 0-.65 1.55A3.59 3.59 0 0 0 5 8.2A8.32 8.32 0 0 0 8.19 11c.44.19.78.3 1.05.39a2.53 2.53 0 0 0 1.17.07a1.93 1.93 0 0 0 1.26-.88a1.67 1.67 0 0 0 .11-.88c-.05-.07-.17-.12-.36-.21z" />
                        <path fill="#4D9FA3" d="M13.29 2.68A7.36 7.36 0 0 0 8 .5a7.44 7.44 0 0 0-6.41 11.15l-1 3.85l3.94-1a7.4 7.4 0 0 0 3.55.9H8a7.44 7.44 0 0 0 5.29-12.72zM8 14.12a6.12 6.12 0 0 1-3.15-.87l-.22-.13l-2.34.61l.62-2.28l-.14-.23a6.18 6.18 0 0 1 9.6-7.65a6.12 6.12 0 0 1 1.81 4.37A6.19 6.19 0 0 1 8 14.12z" /></svg
                ></template>
            </Button>
        </a>
    </div>
</template>

<script setup>
import TitleCard from "../TitleCard.vue";
import Button from "../Button.vue";
</script>
