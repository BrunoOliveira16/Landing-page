<template>
    <button @click="clearValues">Limpar</button>
</template>

<script setup>
    const props = defineProps({
        clearValues: Function,
    })
</script>

<style scoped>
    button {
        width: 100%;
        margin-top: 1rem;
        padding: 5px;
        cursor: pointer;
    }
</style>