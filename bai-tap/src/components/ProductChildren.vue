<template>
    <div>
        <h4>Dữ liệu trong component con</h4>
        <p>id:{{props.idProduct  }}</p>
        <p>ProductName: {{ props.nameProduct }}</p>
        <p>Price: {{ props.priceProduct }}</p>
        <p>Quantity: {{ props.quantityProduct }}</p>
    </div>
</template>

<script setup>
    const props=defineProps(["idProduct","nameProduct","priceProduct","quantityProduct"])
</script>

<style>

</style>