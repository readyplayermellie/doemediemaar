<template>
    <nav class="p-4 text-right">
        <NuxtLink v-for="(item, index) in navLinks" :to="item.url" :key="index" class="p-2">{{ item.title }}</NuxtLink>
    </nav>
    <header class="flex justify-center items-center" id="header">
        <img src="../assets/images/gift-without-background.png">
        <div>
            <MainTitle :title="mainTitle"/>
            <p>{{ subTitle }}</p>
            <div class="flex flex-col">
                <label for="heading-question">{{ headerQuestion }}</label>
                <div>
                    <input type="text" name="heading-question" id="heading-question" class="w-80">
                    <button class="btn btn-primary">{{ searchButton }}</button>
                </div>
            </div>
        </div>
    </header>
</template>

<script setup lang="ts">
import { ref } from 'vue';
const navLinks = ref([
    {
        title: 'Thuis',
        url: '/'
    },
    {
        title: 'Alle lijstjes',
        url: '/all-lists'
    },
    {
        title: 'Over',
        url: '/over'
    }
]);
const mainTitle = ref('De Kadoos');
const subTitle = ref('Jouw cadeau-maatje met cadeau-ideeën voor werkelijk iedereen in je leven, van je lieve oma tot die ene lastige collega.');
const headerQuestion = ref('Voor wie wil je een cadeautje kopen?');
const searchButton = ref('Zoek');
</script>

<style scoped>
#header {
    height: 70%;
    margin: 0% 15% 0% 10%;
}

</style>