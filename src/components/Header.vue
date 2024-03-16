<template>
    <div class="header">
           <img src="../assets/logo.svg"  class="header__icon" />
           <h1 class="header__title">Ignite Feed</h1>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<style scoped lang="scss">
    .header {
        background-color: #202024;
        display: flex;
        padding: 20px;
        align-items: center;
        justify-content: center;

        &__icon {
            margin-right: 1rem;
        }
    
        &__title {
            color: #fff;
            font-weight: bold;
            letter-spacing: 0;
        }
    }
</style>
