<template>
    <div class="w-[200px] h-[200px] rounded-full overflow-hidden flex items-center justify-center">
        <NuxtImg :src="src" :alt="alt" class="object-cover w-full h-full" />
    </div>
</template>

<script setup>
    defineProps({
        src: String,
        alt: {
            type: String,
            default: 'image'
        }
    })
</script>
