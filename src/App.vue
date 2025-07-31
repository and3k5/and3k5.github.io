<script setup lang="ts">
import { ref } from "vue";

const r = ref(180);

setInterval(() => (r.value += -360 + Math.random() * (360 * 2)), 333);
</script>

<template>
    Yo.<br />
    <span class="smiley" :style="{ transform: 'rotate(' + r + 'deg)' }">🤪</span>
</template>

<style scoped>
.smiley {
    display: inline-block;
    transition: transform 400ms linear;
}
</style>
