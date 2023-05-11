<script setup>
import ApplicationLogo from '@/Components/ApplicationLogo.vue';
import PlatformList from "./PlatformList.vue";
</script>

<template>
    <div>
        <div class="p-6 lg:p-8 bg-white border-b border-gray-200">
            <ApplicationLogo class="block h-12 w-auto" />
        </div>

        <div class="bg-gray-100">
            <PlatformList :table-data="[
                {
                    name: 'Example 1',
                    numProjects: 5,
                    numUsers: 10,
                    managePlatform: 'Link 1',
                },
                {
                    name: 'Example 2',
                    numProjects: 3,
                    numUsers: 8,
                    managePlatform: 'Link 2',
                }
            ]"/>
        </div>
    </div>
</template>
