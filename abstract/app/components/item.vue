<template>
    <div class="flex gap-6">
        <Icon 
            :name="icon"
            size="100" 
        />
       <div class="flex flex-col gap-4">
            <h2 class="font-bold text-2xl">
                {{ title }}
            </h2>
            <p class="text-2xl text-wrap">
                {{ description }}
            </p>
            <NuxtLink to="/" class="text-[#4c5FD5] flex gap-2 items-center">
                <span> Learn More </span>
                <Icon name="heroicons-solid:arrow-right"
                />
            </NuxtLink>
       </div> 
    </div>
</template>
<script lang="ts" setup>
defineProps<{
    icon: string,
    title: string,
    description: string,
}>()

</script>