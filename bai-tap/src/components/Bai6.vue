<template>
    <div>
        <h4>Bài 6</h4>
        <Card>
            <template v-slot:header>
                Thông tin sản phẩm
            </template>
            <template v-slot:body>
                Đây là mô tả ngắn gọn về sản phẩm này
            </template>
            <template v-slot:footer>
                <button>Xem chi tiết</button>
            </template>
        </Card>
    </div>
</template>

<script setup>
import Card from './Card.vue'
</script>

<style scoped>
button{
    background-color: brown;
    color: white;
    padding: 5px;
    border-radius: 5px;
    border: transparent;
}
</style>