<template>
    <ChildrenComponent :prop-name="parentData"/>
</template>

<script setup>
import ChildrenComponent from "./ChildrenComponent.vue"
    const parentData='Rikkei Academy'
</script>

<style>

</style>