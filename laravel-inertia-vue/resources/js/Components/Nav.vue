<template>
    <nav class="mt-6">
        <ul class="list-disc">
            <li>
                <inertia-nav-link href="/" :active="$page.component === 'Home'">HomeLink</inertia-nav-link>
            </li>
            <li>
                <inertia-nav-link href="/settings" :active="$page.component === 'Settings'">Settings</inertia-nav-link>
            </li>
            <li>
                <inertia-nav-link href="/users" :active="$page.component === 'Users'">Users</inertia-nav-link>
            </li>
            <li>
                <button @click="handleLogout" class="text-blue-500 hover:underline"
                >Log Out
                </button>
            </li>
        </ul>
    </nav>
</template>
<script setup lang="ts">
import {Inertia} from '@inertiajs/inertia';
import InertiaNavLink from "@/Components/inertiaNavLink.vue";

const handleLogout = () => {
    Inertia.post('/logout');
};
</script>
