<template>
     <button @click="deleteI">Delete</button>
</template>

<script setup>
    const emit=defineEmits(['deleteId']);
    const deleteI=()=>{
        emit('deleteId',1);
    }

</script>

<style>

</style>