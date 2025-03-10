<template>
    <div class="rounded-xl m-4" id="item-card">
        <img src="../assets/images/gift-with-background.jpeg">
        <div class="p-3">
            <h3>{{ title }}</h3>
            <p>{{ content }}</p>
        </div>
    </div>
</template>

<script setup lang="ts">
const props = defineProps({
    title: String,
    content: String,
})
</script>

<style scoped>
#item-card {
    border: 1px solid black;
    background-color: white;
}

img {
    border-radius: 10px 10px 0px 0px;
    border-bottom: 1px solid black;
}
</style>