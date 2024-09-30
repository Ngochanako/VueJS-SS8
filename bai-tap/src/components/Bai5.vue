<template>
   <div>
      <h4>Bài 5</h4>
       <Modal v-if="showModal" @close="closeModal">
        <template v-slot:header>
            <h2>Thông báo từ hệ thống</h2>
        </template>
        <p>Đây là nội dung của modal. Bạn có thể đóng modal bằng cách nhấn vào nút 'Close'.</p>
       </Modal>
   </div>
</template>

<script setup>
import { ref } from 'vue';
import Modal from './Modal.vue';
const showModal=ref(true);
const closeModal=()=>{
    showModal.value=false;
}
</script>

<style>

</style>