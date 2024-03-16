<template>
    <div class="header">
           <img src="../assets/logo.svg" />
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>
