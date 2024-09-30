<template>
    <div>
        <button type="typeButton" @click="messageClick">
           <slot></slot>
        </button>
    </div>
</template>

<script setup>
const emit=defineEmits(['click']);
const messageClick=()=>{
    emit('click');
}
const props=defineProps({
    type:String
})
</script>

<style scoped>
button{
    background-color: brown;
    color: white;
    padding: 5px;
    border-radius: 5px;
    border:transparent;
}

</style>