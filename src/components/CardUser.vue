<template>
    <div class="card">
        <img src="data:image/jpeg;base64,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" class="card__background"/>
        <div class="card__content">
            <h1 class="card__content-user">Demetrius Leonardo</h1>
            <p class="card__content-role">Software Developer</p>   
        </div>
        <div class="card__footer">
                <button class="card__footer--action">
                <img src="../assets/edit-user.svg" />
                    Editar seu perfil
                </button>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<style scoped lang="scss">
    .card {
        height: 256px;
        width: 294px;
        background: #202024;
        border-radius: .5rem;
        margin-top: 2rem;
        display: flex;
        flex-direction: column;

        &__background {
            max-height: 72px;
            width: 294px;
        }
    
        &__content {
            display: flex;
            justify-content: certer;
            flex-direction: column;
            align-items: center;
            border-bottom: 1px solid #323238;
            height: 40%;

            &-user {
                color: #E1E1E6;
                font-size: 1rem;
                font-weight: bold;
                text-align: center;
                margin-bottom: 5px;
                margin-top: 40px;
            }
        
            &-role {
                color: #8D8D99;
                font-size: .8rem;
                font-weight: 500;
                text-align: center;

            }
        }
    
        &__footer{
            display: flex;
            align-items: center;
            &--action {
                padding: 20px 25px;
                margin-top: 10px;
                background: none;
                border: 1px solid #00B37E;
                margin-left: auto;
                margin-right: auto;
                color: #00B37E;
                border-radius: 8px;
            }
            img {
                position: relative;
                top: 3px;
                margin-right: 10px;
            }
        }
    }
</style>
