<template>
  <div>
    <p>Giá trị ô input:{{ inputValue }}</p>
    <BaseInput @value-input="handleInput" type="text" placeholder="Enter...."  modal-vl=''>
        <p>Slot</p>
    </BaseInput>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import BaseInput from './BaseInput.vue';
const inputValue=ref('');
const handleInput=(value)=>{
    inputValue.value=value;
}
</script>

<style>

</style>