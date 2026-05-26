<script setup>
import { ref, computed } from 'vue';

const props = defineProps({
    details: {
        type: Array,
        required: true
    }
})

</script>

<template>
    <ul>
        <li v-for="detail in details">{{ detail }}</li>
    </ul>
</template>