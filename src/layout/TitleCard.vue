<template>
    <div :class="className" class="text-primary">
        <h2 class="text-[2.2rem] flex items-center gap-3">
            <img class="w-10 h-10" v-if="src" :src="src" alt="src"> <slot></slot>
        </h2>
        <div class="border-b border-accent w-25"></div>
    </div>
</template>

<script setup>
defineProps({
    src: String,
    className: String
})
</script>