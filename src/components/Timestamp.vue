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
    <span class="timestamp">{{props.timestamp}}</span>
</template>

<style>
</style>