<template>
    <h1>Welcome Page {{ name }}</h1>
    <div v-for="framework in frameworks" :key="framework">
        {{ framework }}
    </div>
</template>

<script setup>
defineProps({
    name: String,
    frameworks: Array,
})

</script>
