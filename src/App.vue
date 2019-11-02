<template>
    <div class="container">
      <app-header></app-header>
      <app-new-quote @quoteAdded='newQuote'></app-new-quote>
      <app-quoute-grid :quotes='quotes' @deletedQuote='deleteQuote'></app-quoute-grid>
      <div class="row">
        <div class="col-sm-12 text-center">
            <div class="alert alert-info">
              Info: Click on a Quote to delete it.
            </div>
        </div>
      </div>
    </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';
import NewQuote from './components/NewQuote.vue';
import Header from './components/Header.vue';
    export default {
        data: function(){
          return {
              maxQuotes: 10,
              quotes:[" It is just quote to see something"]
          };
        },
        methods:{
          newQuote(quote){
            this.quotes.push(quote);
              console.log('New Quote is:',quote);
          },
          deleteQuote(index){
            this.quotes.splice(index,1);
          }
        },
        components:{
          appQuouteGrid: QuoteGrid,
          appNewQuote: NewQuote,
          appHeader: Header
        }
    }
</script>

<style>
</style>
