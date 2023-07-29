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
        <img :src="props.image" class="profile" alt="profile" />
</template>

<style>
</style>