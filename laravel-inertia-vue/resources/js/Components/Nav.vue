<template>
    <nav>
        <ul>
            <li>
                <Link href="/">Home</Link>
            </li>
            <li>
                <Link href="/settings">Settings</Link>
            </li>
            <li>
                <Link href="/users">Users</Link>
            </li>
        </ul>
    </nav>
</template>
<script setup lang="ts">
import {Link} from "@inertiajs/vue3";
</script>
