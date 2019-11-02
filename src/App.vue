<template>
    <div class="container">
      <app-quoute-grid :quotes='quotes'></app-quoute-grid>
    </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';
    export default {
        data: function(){
          return {
              maxQuotes: 10,
              quotes:[" It is just quote to see something"]
          };
        },
        components:{
          appQuouteGrid: QuoteGrid
        }
    }
</script>

<style>
</style>
