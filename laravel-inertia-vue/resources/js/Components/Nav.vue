<template>
    <nav class="mt-6">
        <ul class="list-disc">
            <li>
                <Link href="/">Home</Link>
            </li>
            <li>
                <Link href="/settings">Settings</Link>
            </li>
            <li>
                <Link href="/users">Users</Link>
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
import {Link} from "@inertiajs/vue3";
import {Inertia} from '@inertiajs/inertia';

const handleLogout = () => {
    Inertia.post('/logout');
};
</script>
