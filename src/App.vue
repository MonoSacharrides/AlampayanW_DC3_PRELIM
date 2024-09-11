<script>
import Item from './components/Item.vue'
import ItemList from './components/ItemList.vue'

export default {
  name: 'App',
  components: { ItemList, Item },
  data() {
    return {
      products: [
        { id: 1, name: 'Item 1', price: 20 },
        { id: 2, name: 'Item 2', price: 50 },
        { id: 21, name: 'Item 3', price: 100 }
      ],
      product: { id: 3, name: 'Product 3', price: 50 }
    }
  }
}
</script>

<template>
  <div class="app">
    <h1></h1>
    <ItemList :products="products" />
  </div>
</template>

<style scoped>
body{
  display: flex;
  color: black;
}
.app {
  font-family: Arial, sans-serif;
  margin: 20px;
  text-align: center;
  font-size: 30%;
}

h1 {
  color: #000000FF;
  font-size: 24px;
  margin-bottom: 20px;
}
</style>
