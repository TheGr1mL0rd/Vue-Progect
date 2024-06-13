// Счетчик боллее читабельней 
<script setup>
defineProps({
        title: String,
        price: Number,
        isAdded: Boolean
    });
</script>

<template>
    <div class="product">
        <h2>Товар: {{ title }}</h2>
        <h3>Цена: {{ price }}</h3>
        <h3>Цена: {{ isAdded }}</h3>
    <slot></slot>
    </div>
</template>

<style scoped>
    .product {
        border: 2px solid blue;
        padding: 10px;
        margin-bottom: 10px;
    }

    .header {
        border: 2px solid black;
        padding: 5px;
        margin-bottom: 5px;
    }

    
</style>