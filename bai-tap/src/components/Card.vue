<template>
     <div class="container">
        <header class="header">
           <slot name="header"></slot>
        </header>
        <hr>
        <div>
            <slot name="body"></slot>
        </div>
        <hr>
        <footer>
            <slot name="footer"></slot>
        </footer>
     </div>
</template>

<script setup>
     
</script>

<style scoped>
.container{
    width: 200px;
    display: flex;
    flex-direction: column;
    gap:10px;
    border:1px solid rgb(203, 194, 194);
    border-radius: 5px;
    padding: 10px;
}
.header{
    font-size: 18px;
    font-weight: bold;
}
hr{
    color: brown;
}

</style>