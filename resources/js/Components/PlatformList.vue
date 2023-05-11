<script setup>

defineProps({
    tableData: Array,
});
</script>
<template>
    <div class="p-2">
        <table class="w-full">
            <thead>
            <tr class="border-b-2">
                <th class="text-left pl-2">Name</th>
                <th class="text-center">Number of Projects</th>
                <th class="text-center">Number of Users</th>
                <th class="text-center">Manage Platform</th>
            </tr>
            </thead>
            <tbody>
            <tr v-for="item in tableData" :key="item.name" class="bg-white">
                <td class="text-left pl-2">{{ item.name }}</td>
                <td class="text-center">{{ item.numProjects }}</td>
                <td class="text-center">{{ item.numUsers }}</td>
                <td class="text-center">{{ item.managePlatform }}</td>
            </tr>
            </tbody>
        </table>
    </div>
</template>

