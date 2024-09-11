<script>
export default {
name: 'Item',
props: ['product'],
components: ['product'],
methods: {
    addToCart(product) {
    console.log(product)
    }
}
}
</script>

<template>
<div class="item">
    <h3>{{ product.name }}</h3>
    <p>Price: {{ product.price }}</p>
    <button @click="addToCart(product)">Add to Cart</button>
</div>
</template>
<style scoped>
button{
    border: 1px solid black;
    border-radius: 5px;
    width: 110px;
    height: 30px;
    font-weight: bold;
}
button:hover{
    color: rgb(0, 0, 0);
    background-color: aqua;
}


.list-container {
color: #000000FF;
font-size: 24px;
margin-bottom: 20px;
border: 1px solid black;
border-radius: 5px;
align-items: center;
}
</style>
