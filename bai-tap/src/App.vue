<script setup>
     import ParentComponent from "./components/ParentComponent.vue";
     import ProductComponent from "./components/ProductParent.vue";
     import CountParent from "./components/CountParent.vue"
     import TodoApp from './components/TodoApp.vue'
     import Bai5 from './components/Bai5.vue'
     import Bai6 from './components/Bai6.vue'
     import MessageParent from './components/MessageParent.vue'
     import ListUser from './components/ListUser.vue'
     import Bai9 from './components/Bai9.vue'
     import Bai10 from './components/Bai10.vue'
</script>

<template>
     <div>
     <h4>Bài 1</h4>
     <ParentComponent/>
     <h4>Bài 2</h4>
     <ProductComponent/>
     <CountParent/>
     <TodoApp/>
     <Bai5/>
     <Bai6/>
     <h4>Bài 7</h4>
     <MessageParent/>
     <h4>Bài 8</h4>
     <ListUser/>
     <h4>Bài 9</h4>
     <Bai9/>
     <h4>Bài 10</h4>
     <Bai10/>
    </div>
</template>

<style scoped>

</style>
