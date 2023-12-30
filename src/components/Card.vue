<template>
    <div class="card" :class="hasPadding && 'hasPad'">
        <h3 class="title">{{ heading }}</h3>
        <p class="text">{{ text }}</p>
    </div>
</template>
<script setup lang="ts">

defineProps({
    heading: String,
    text: String,
    hasPadding: Boolean
})
</script>
<style scoped>
.card {

    border: 2px solid #cef;
}
.hasPad{
    padding: 20px;
}

</style>