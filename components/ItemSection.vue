<template>
    <section>
        <SectionTitle :title="title" />
        <div class="flex m-4">
            <SingleItem v-for="(item, index) in popularProducts" :title="item.title" :content="item.content" :key="index" />
        </div>
    </section>
</template>

<script setup lang="ts">
const props = defineProps({
    title: String,
});
import { ref } from 'vue';
const popularProducts = ref([
    {
        title: 'Doe maar wat',
        content: 'Cadeau-ideeën voor mensen die altijd zeggen ‘Doe maar wat’'
    },
    {
        title: 'Puppy',
        content: 'Cadeau-ideeën voor goede vrienden die net een puppy in huis hebben genomen'
    },
    {
        title: 'Collega',
        content: 'Cadeau-ideeën voor collega’s die nooit taart mee naar kantoor nemen'
    }
]);

const newestProducts = ref([
    {
        title: 'Doe maar wat',
        content: 'Cadeau-ideeën voor mensen die altijd zeggen ‘Doe maar wat’'
    },
    {
        title: 'Puppy',
        content: 'Cadeau-ideeën voor goede vrienden die net een puppy in huis hebben genomen'
    },
    {
        title: 'Collega',
        content: 'Cadeau-ideeën voor collega’s die nooit taart mee naar kantoor nemen'
    }
]);
</script>