<template>
    <div>
        <h4>Bài 3</h4>
        <p>Count:{{ count }}</p>
        <CountChildrent @increment="handleIncrement"/>
    </div>
</template>

<script setup>
import CountChildrent from "./CountChildren.vue"
import {ref } from "vue";
const count=ref(0);
const handleIncrement=()=>{
    count.value++;
}
</script>

<style>

</style>