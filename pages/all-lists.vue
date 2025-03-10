<template>
    <Banner>
        <div class="flex flex-col">
            <label for="heading-question">{{ headerQuestion }}</label>
            <div>
                <input type="text" name="heading-question" id="heading-question" class="w-80">
                <button class="btn btn-primary">{{ searchButton }}</button>
            </div>
        </div>
    </Banner>
    <section>
        <SectionTitle :title="allProductsTitle" />
    </section>
</template>

<script setup lang="ts">
const headerQuestion = ref('Voor wie wil je een cadeautje kopen?');
const searchButton = ref('Zoek');
const allProductsTitle = ref('De cadeaulijstjes');
</script>