<template>
    <div class="container">

    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<style scoped lang="scss">
    .container {
        max-height: 621px;
        max-width: 830px;
        border-radius: 8px;
        background: #323238;
        padding: 40px;
    }
</style>
