<template>
  <div>
    <h1>Stocks</h1>
    <div class="row">
      <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
    </div>
  </div>
</template>

<script>
  import Stock from '../stocks/Stock.vue';

  export default {
    data() {
      return {
        stocks: [
          { id: 1, name: 'BMW', price: 100 }, 
          { id: 2, name: 'Google', price: 200 }, 
          { id: 3, name: 'Apple', price: 210 },
          { id: 3, name: 'Twitter', price: 80 },
        ]
      }
    },
    components: {
      appStock: Stock
    }
  }
</script>

<style>
  
</style>
