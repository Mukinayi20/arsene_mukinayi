<template>
    <div class="p-6 m-5 border-xl border border-primary/10 rounded-2xl bg-bgPrimary dark:bg-[#151b1f] dark:hover:border-accent/20" :class="autherClass">
        <slot></slot>
    </div>
</template>

<script setup>
defineProps({
    autherClass: String
})
</script>