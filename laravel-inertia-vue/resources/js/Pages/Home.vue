<template>
    <h1>Welcome Page {{ name }}</h1>
    <ul class="list-disc pl-5">
        <li v-for="framework in frameworks" :key="framework">
            {{ framework }}
        </li>
    </ul>
</template>

<script setup>
defineProps({
    name: String,
    frameworks: Array,
})

</script>
