<template>
    <header class="sticky top-0 bg-weather-primary shadow-lg">
        <nav class="container flex flex-col sm:flex-row items-center gap-4 text-white py-6">
            <RouterLink :to="{ name: 'home' }">
                <div class="flex items-center gap-3 flex-1 text-2xl">
                    <font-awesome-icon :icon="['fas', 'sun']" />
                    <p class="text-2xl">The Weather App</p>
                </div>
            </RouterLink>

            <div class="flex gap-3 flex-1 justify-end text-2xl">
                <font-awesome-icon :icon="['fas', 'circle-info']" />
                <font-awesome-icon :icon="['fas', 'plus']" />
            </div>

            <BaseModal>
                <h2 class="text-black">Test</h2>
            </BaseModal>
        </nav>
    </header>
</template>

<script setup>
    import { RouterLink } from 'vue-router'
    import BaseModal from './BaseModal.vue'
</script>

<style lang="scss" scoped></style>