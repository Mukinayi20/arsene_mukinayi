<template>
    <div id="projet" class="bg-bgMesprojet flex justify-center">
        <div class="dark:bg-[#151b1f] p-8 max-lg:p-0 pb-25 flex flex-col items-center">
            <div class="w-[75%]">
                <TitleCard className="flex items-start flex-col gap-5 mt-5">Projets Sélectionnés</TitleCard>
                <div class="z-1">
                    <ComposantProjet></ComposantProjet>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import TitleCard from "../../layout/TitleCard.vue";
import ComposantProjet from "./ComposantProjet.vue";
</script>
