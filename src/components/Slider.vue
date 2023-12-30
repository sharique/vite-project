<script setup lang="ts">

import { ref } from 'vue';
const value = ref(0)
defineProps(['name'])
</script>

<template>
    <div>
        <h3>
            {{ $props.name }}
        </h3>
        <input type="range" v-model="value" />
        <div class="test">{{ value }}</div>
    </div>
</template>