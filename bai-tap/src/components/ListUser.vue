<template>
    <div>
        <button @click="showModal=true">Add user</button>
        <FormAddUser @close-modal="showModal=false" :is-visible="showModal"/>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import FormAddUser from './FormAddUser.vue'
const showModal=ref(false);
</script>

<style scoped>
button{
    background-color: brown;
    color: white;
    padding: 5px;
    border-radius: 5px;
    border:transparent;
}
</style>