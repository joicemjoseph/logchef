<script setup lang="ts">
// LogsLayout component - provides consistent layout for log-related views
</script>

<template>
    <router-view v-slot="{ Component }">
        <keep-alive :include="['LogExplorer']">
            <component :is="Component" />
        </keep-alive>
    </router-view>
</template>