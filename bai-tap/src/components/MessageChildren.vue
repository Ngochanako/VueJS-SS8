<template>
    <div>
        <button @click="sendMessage">Send Message</button>
    </div>
</template>

<script setup>
const emit=defineEmits(['message']);
const sendMessage=()=>{
    emit('message', 'Welcome to Rikkei!'); 
}
</script>

<style>

</style>