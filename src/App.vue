<template>
  <div class="container">
    <app-new-quote @quoteAdded="NewQuote"></app-new-quote>
    <appQuoteGrid :quotes="quotes"></appQuoteGrid>
  </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue';
import NewQuote from './components/NewQuote.vue';

export default {
  data: function() {
    return {
      quotes:[
        'Just a Quote to see something'
      ],
      maxQuotes: 10
    }
  },
  methods: {
    NewQuote(quote){
      this.quotes.push(quote);
    }
  },
  components: {
    appQuoteGrid: QuoteGrid,
    appNewQuote: NewQuote
  }
}
</script>

<style lang="scss" scoped>
  
</style>
