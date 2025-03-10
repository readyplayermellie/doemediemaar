<template>
    <section>
        <SectionTitle :title="contactTitle" />
        <form class="flex flex-col justify-between pt-6">
            <div class="flex justify-between">
                <label for="name">Naam</label>
                <input type="text" name="name" id="name" class="contact-input">
            </div>
            <div class="flex justify-between">
                <label for="email">E-mailadres</label>
                <input type="email" name="email" id="email" class="contact-input">
            </div>
            <div class="flex justify-between">
                <label for="suggestion">Jouw suggestie</label>
                <input type="text" name="suggestion" id="suggestion" class="contact-input">
            </div>
            <div class="flex justify-end">
                <button class="btn btn-primary">Verstuur</button>
            </div>
        </form>
    </section>
</template>

<script setup lang="ts">
const contactTitle = ref('Ideeënbox');
</script>

<style scoped>
form {
    margin: 0px 15%;
}

button {
    margin-top: 20px;
}
</style>