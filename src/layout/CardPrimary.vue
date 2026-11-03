<template>
    <div class="bg-secondary w-max p-3 rounded-lg">
        <img v-if="icone" :src="icone" alt="icone" class="w-10">
    </div>
</template>

<script setup>
defineProps({
    icone: String
})
</script>