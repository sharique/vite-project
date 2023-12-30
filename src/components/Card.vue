<template>
    <div class="card">
        <h3 class="title">{{ heading }}</h3>
        <p class="text">{{ text }}</p>
    </div>
</template>
<script setup lang="ts">

defineProps({
    heading: String,
    text: String
})
</script>
<style scoped>
.card {
    padding: 10px;
    border: 2px solid #cef;
}
</style>