<template>
     <div>
        <h4>Bài 4</h4>
        <p>Id to delete:{{ id }}</p>
        <TodoItem @delete-id="handleId"/>
     </div>
</template>

<script setup>
    import { ref } from 'vue';
import TodoItem from './TodoItem.vue';
    const id = ref(null);
    const handleId=(idDelete)=>{
        id.value = idDelete;
    }
</script>

<style>

</style>