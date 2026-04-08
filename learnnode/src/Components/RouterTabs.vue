<script setup>
import { computed } from 'vue';
import { useRoute, useRouter } from 'vue-router';

const route = useRoute();
const router = useRouter();

const routes = computed(() =>
    router
        .getRoutes()
        .filter(r => typeof r.name === 'string' && r.path)
);
</script>

<template>
    <div class="tabs is-centered">
        <ul>
            <li
                v-for="item in routes"
                :key="item.path"
                :class="{ 'is-active': route.path === item.path }"
            >
                <RouterLink :to="item.path">{{ item.name }}</RouterLink>
            </li>
        </ul>
    </div>
</template>