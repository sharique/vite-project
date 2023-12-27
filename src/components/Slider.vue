<script setup lang="ts">

import {ref} from 'vue';
const value = ref(0)
</script>

<template>
    <h3>
        Slider
    </h3>
    <input type="range" v-model="value" />
    <div class="test">{{ value }}</div>
</template>