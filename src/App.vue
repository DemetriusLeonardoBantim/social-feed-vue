<script setup lang="ts">
  import Header from './components/Header.vue'
  import CardUser from './components/CardUser.vue'
  import Posts from './components/Posts.vue'
</script>

<template>
  <div class="container">
    <Header class="container__header" />
    <div class="container-body">
        <CardUser class="container-body__card" />
        <Posts class="container-body__posts"/>
    </div>
  </div>
</template>


<style scoped lang="scss">
  .container {
    background: #121214;
    height: 100vh;
    &-body {
      display: flex;
      justify-content: space-evenly; 
    
      &__posts {
        flex: 1;
        margin-top: 2rem;
      }
    
      &__posts {
        margin-top: 2rem;
      }
    }
  }
</style>