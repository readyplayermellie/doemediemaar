<template>
    <div class="relative">
        <h1 class="z-10 relative">{{ title }}</h1>
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
    width: 500px;
    height: 25px;
    bottom: 20px;
    left: 20px;
}
</style>