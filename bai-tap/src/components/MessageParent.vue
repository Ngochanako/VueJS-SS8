<template>
    <div>
        <MessageChildren @message="handleMessage"/>
    </div>
</template>

<script setup>
import MessageChildren from './MessageChildren.vue';
const handleMessage=(msg)=>{
    alert(msg);
}
</script>

<style>

</style>