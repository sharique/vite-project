<template>
    <div class="card" :class="[hasMargin? 'hasMargin': '', hasPadding? 'hasPad': '']" >
        <h3 class="title">{{ heading }}</h3>
        <p class="text">{{ text }}</p>
    </div>
</template>
<script setup lang="ts">

defineProps({
    heading: String,
    text: String,
    hasPadding: Boolean,
    hasMargin: Boolean
})
</script>
<style scoped>
.card {

    border: 2px solid #cef;
}

.hasPad {
    padding: 20px;
}

.hasMargin {
    margin: 10px;
}
</style>