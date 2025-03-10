<template>
    <div class="relative">
        <h2 class="z-10 relative">{{ title }}</h2>
        <div id="backline" class="absolute"></div>
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
    title: String,
});
</script>

<style scoped>
#backline {
    background-color: #A1E99F;
    width: 100%;
    height: 25px;
    bottom: 2px;
    left: 20px;
}
</style>