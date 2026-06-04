<template>
    <div class="flex justify-between h-20 py-6 px-10 border-b border-b-gray-200">
        <div class="flex gap-6">
            <div class="flex">
                <Menu :size="30"/>
                <Columns3 :size="30"/>
            </div>
            <div class="flex gap-6">    
                <NuxtLink to="/"> Live </NuxtLink>
                <NuxtLink to="/"> Push </NuxtLink>
                <NuxtLink to="/"> Link </NuxtLink>
                <NuxtLink to="/"> Shop </NuxtLink>
                <NuxtLink to="/"> Packs </NuxtLink>
                <NuxtLink to="/"> Help </NuxtLink>
                <NuxtLink class="flex items-center h-6" to="/"> 
                    More
                    <Plus :size="18"/>
                </NuxtLink>
            </div>
        </div>
        <div class="flex gap-4">
            <NuxtLink class="text-[#0000FF]" to="/"> Try Live for free </NuxtLink>
            <NuxtLink to="/"> Account </NuxtLink>
            <NuxtLink to="/"> Log out <output></output> </NuxtLink>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { Columns3, Menu, Plus } from '@lucide/vue';

</script>