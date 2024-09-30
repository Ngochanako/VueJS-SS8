<template>
    <div class="container">
        <BaseButton type="submit" @click="handleSubmit">
            Submit
        </BaseButton>
        <BaseButton type="button" @click="handleCancel">
            Cancel
        </BaseButton>
        <BaseButton type="reset" @click="handleReset">
            Reset
        </BaseButton>
    </div>
</template>

<script setup>
import BaseButton from './BaseButton.vue'
const handleCancel=()=>{
    alert("Cancel")
}
const handleReset=()=>{
    alert("Reset")
}
const handleSubmit=()=>{
    alert("Submit")
}
</script>

<style scoped>
.container{
    display: flex;
    gap: 20px;
}
</style>