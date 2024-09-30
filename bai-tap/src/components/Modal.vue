<template>
    <div class="container">
        <header class="header">
            <slot name="header"></slot>
        </header>
        <hr>
        <p>
           <slot></slot>
        </p>
        <hr>
        <button @click="closeModal">Close</button>
    </div>
</template>

<script setup>
const emit=defineEmits(['close']);
const closeModal=()=>{
    emit('close');  
}  
</script>

<style scoped>
.container {
   display: flex;
   flex-direction: column;
   gap:10px;
   border: 1px solid rgb(211, 204, 204);
   padding: 10px;
   width: 300px;
}
.header{
    font-size: 18px;
    font-weight: bold;
}

</style>