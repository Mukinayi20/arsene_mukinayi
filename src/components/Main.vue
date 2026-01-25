<template>
    <div>
        <Apropos/>
        <MesProjets/>
        <Temoignage/>
        <Collaboration/>
        <!-- <Soutien/> -->
    </div>
</template>

<script setup>
import MesProjets from './projet/MesProjets.vue';
import Apropos from './apropos/Apropos.vue';
import Temoignage from './Temoignage.vue';
import Collaboration from './collaboration/Collaboration.vue';
import Soutien from './soutien/Soutien.vue';
</script>