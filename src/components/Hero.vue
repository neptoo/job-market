<template>
    <section class="sec-gradient py-20 mb-4">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col items-center">
            <div class="text-center">
                <h1 class="font-serif text-4xl font-extrabold text-green-900 sm:text-5xl md:text-6xl">
                    {{ title }}
                </h1>
                <p class="font-serif my-4 text-xl text-green-900">
                    {{ subtitle }}
                </p>
            </div>
        </div>
    </section>
</template>

<script setup>
import { defineProps } from 'vue';
defineProps({
    title: String,
    subtitle: {
        type: String,
        default: 'Find the Vue job that fits your skills and needs'
    }
})
</script>

<style scoped>
.sec-gradient {
    background-image: linear-gradient(to top, #c1dfc4 0%, #deecdd 100%);
}
</style>
