<script setup>
import RouterTabs from './Components/RouterTabs.vue';
</script>

<template>
    <RouterTabs></RouterTabs>
    <Suspense>
        <RouterView></RouterView>
    </Suspense>
</template>

<style></style>