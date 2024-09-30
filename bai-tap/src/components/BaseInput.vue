<template>
  <div>
    <slot></slot>
    <input @input="messageInput" :type="type" :placeholder="placeholder" :value="modalVl">
  </div>
</template>

<script setup>
const props=defineProps({
    placeholder: {
      type: String,
      required: true
    },
    type:{
        type:String
    },
    modalVl:{
        type:String
    }
})
const emit=defineEmits(['valueInput']);
const messageInput=(event)=>{
    emit('valueInput',event.target.value);
}
</script>

<style>
input{
    width: 300px;
    padding: 10px;
    margin-top: 10px;
    border: none;
    border-bottom: 1px solid #ccc;
}
</style>