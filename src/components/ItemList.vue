<script>
import Item from './Item.vue'
export default {
name: 'ItemList',
props: ['products'],
components: { Item },
data() {
    return {}
},
methods: {}
}
</script>

<template>
<div class="product-list">
    <h2>Items List</h2><br>
    <div class="list-container">
    <Item v-for="product in products" :key="product.id" :product="product" />
    </div>
</div>
</template>
<style scoped>
h2{
    font-size: 50px;
    font-weight: bold;
}


.list-container {
color: #FFFFFFFF;
font-size: 24px;
margin-bottom: 20px;
border: 1px solid black;
border-radius: 5px;
align-items: center;
display: flex;
width: 100%;
background-color: black;
left: 50px;
}
</style>

