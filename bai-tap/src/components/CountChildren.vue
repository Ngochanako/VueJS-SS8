<template>
    <div>
      <button @click="increment">Increment</button>
    </div>
  </template>
  
  <script setup>

  const emit = defineEmits(['increment']);
  
  const increment = () => {
    emit('increment');
  };
  </script>
  
  <style scoped>
  button {
    padding: 10px;
    font-size: 16px;
    cursor: pointer;
  }
  </style>
  