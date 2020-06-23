<template>
  <div>
    <div class="conatiner">
      <div class="row">
        <div class="col-sm-6 offset-sm-3">
          <div class="card mt-5">
            <div class="card-body">
              <div class="card-text">
                <h3 class="quote">"{{ quote }}"</h3>
                <p class="author">- Bob Ross</p>
              </div>
            </div>
          </div>
          <button @click="getQuote" class="btn btn-primary btn-lg">
            New Quote
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import quotes from '../quotes';

export default {
  name: 'QuoteMachine',
  data() {
    return {
      quote: quotes[0],
    };
  },
  methods: {
    getQuote() {
      const quote = quotes[Math.floor(Math.random() * quotes.length)];
      this.quote = quote;
    },
  },
};
</script>

<style>
button {
  margin-left: 40%;
}

.card {
  margin-bottom: 2rem;
}

.quote {
  line-height: 1.5;
  margin-bottom: 2rem;
}

.author {
  font-size: 1.2rem;
  text-align: right;
  margin-right: 2rem;
}
</style>
