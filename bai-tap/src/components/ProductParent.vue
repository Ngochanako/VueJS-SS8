<template>
    <div>
       <ProductChildren :id-product=" product.id " :name-product="product.name" :price-product="product.price" :quantity-product="product.quantity"/> 
    </div>
</template>

<script setup>
import ProductChildren from "./ProductChildren.vue";
const product={
    id:1,
    name:'Product 1',
    price: 10000,
    quantity:10
}   
</script>

<style>

</style>