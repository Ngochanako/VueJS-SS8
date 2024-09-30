<template>
    <div class="container" v-if="isVisible">
        <h2>Form Add user</h2>
        <main>
            <div>Name</div>
            <input type="text">
            <div>Email</div>
            <input type="text">
            <div>Address</div>
            <input type="text">
            <button @click="closeModal">Close</button>
        </main>
    </div>
</template>

<script setup>
const props=defineProps({
    isVisible:Boolean
})
const emit=defineEmits(['closeModal']);
const closeModal=()=>{
    emit('closeModal');
}
</script>

<style scoped>
.container{
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 10px;
    width: 300px;
}
main{
    display: flex;
    flex-direction: column;
    gap: 10px;
}
button{
    background-color: brown;
    color: white;
    padding: 5px;
    border-radius: 5px;
    border:transparent;
}
input{
    width: 100%;
    border: 1px solid rgb(207, 204, 204);
}
</style>