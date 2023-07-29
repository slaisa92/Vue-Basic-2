<script setup>
const props = defineProps ({
        name: String, 
        image: String, 
        handle: String,
        timestamp: String,
        message: String
})
</script>
<template>
    <p class="message">
        {{props.message}}
    </p>
</template>

<style>
</style>