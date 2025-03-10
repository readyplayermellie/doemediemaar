<template>
    <Banner>
        <h2>{{ bannerText }}</h2>
    </Banner>
    <ItemSection v-for="(item, index) in itemSectionContent" :title="item.title" :key="index"/>
    <ContactForm />
</template>

<script setup lang="ts">
import { ref } from 'vue';
const bannerText = ref('“Wat moet ik nou weer kopen” zegt niemand meer');
const itemSectionContent = ref([
    {
        title: 'Populaire cadeaulijstjes',
    },
    {
        title: 'Nieuwe cadeaulijstjes',
    },
]);
</script>