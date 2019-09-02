<template>
  <div>
    <Stock v-for="stock in stocks" :stock="stock" />
  </div>
</template>

<script>
import Stock from './Stock';

export default {
  name: 'Stocks',
  data: function() {
    return {
      stocks: [
        {
          id: 1,
          name: 'BMW',
          price: 110
        },
        {
          id: 2,
          name: 'Google',
          price: 200
        },
        {
          id: 3,
          name: 'Apple',
          price: 250
        },
        {
          id: 4,
          name: 'Twitter',
          price: 8
        }
      ]
    };
  },
  components: {
    Stock
  }
};
</script>
