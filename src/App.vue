<template>
    <div class="container">
      <app-new-quote @quoteAdded='newQuote'></app-new-quote>
      <app-quoute-grid :quotes='quotes'></app-quoute-grid>
    </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';
import NewQuote from './components/NewQuote.vue';
    export default {
        data: function(){
          return {
              maxQuotes: 10,
              quotes:[" It is just quote to see something"]
          };
        },
        components:{
          appQuouteGrid: QuoteGrid,
          appNewQuote: NewQuote
        }
    }
</script>

<style>
</style>
