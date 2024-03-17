<template>
    <div class="card">
        <div class="card__header">
            <img src="https://avatars.githubusercontent.com/u/67908082?v=4" class="card__header-avatar"/>
        </div>
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

        &__header {
            background-image: url('../assets/background.jpeg');
            height: 72px;
            background-size: cover;
            background-position: center;
        
            &-avatar{
                height: 60px;
                width: 60px;
                border: 2px solid #00B37E;
                border-radius: 10px;
                position: relative;
                left: 40%;
                top: 25px;
            }
        }

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
            height: 80px;

            &-user {
                color: #E1E1E6;
                font-size: 1rem;
                font-weight: bold;
                text-align: center;
                margin-bottom: 5px;
                margin-top: 25px;
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
                padding: 10px 25px;
                margin-top: 20px;
                background: none;
                border: 1px solid #00B37E;
                margin-left: auto;
                margin-right: auto;
                color: #00B37E;
                border-radius: 8px;
                cursor: pointer;
            }
            img {
                position: relative;
                top: 3px;
                margin-right: 10px;
            }
        }
    }
</style>
