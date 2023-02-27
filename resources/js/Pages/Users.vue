<template>
    <Head title="Users" />
        <h1 class="text-3xl">Users</h1>

        <ul>
            <li
            v-for="user in users"
            :key="user.id"
            v-text="user.name" />
        </ul>
</template>

<script>
import Layout from "../Shared/Layout.vue";
export default {
    layout: Layout
};
</script>

<script setup>
defineProps({users: Array});
</script>

<!-- <script setup>
import { Head } from "@inertiajs/vue3";
</script>
component is imported globaly this is just an example -->