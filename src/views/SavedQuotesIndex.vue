<template>
  <div class="home">
    <h1>All Saved Quotes</h1>
    <div v-for="saved_quote in saved_quotes" v-bind:key="saved_quote.id">
      <h2>{{ saved_quote.quote }}</h2>
      <img v-bind:src="saved_quote.image_url" v-bind:alt="saved_quote.id" />
      <p>Status: {{ saved_quote.status }}</p>
      <p>Author: {{ saved_quote.author }}</p>
    </div>
  </div>
</template>

<style></style>

<script>
import axios from "axios";
export default {
  data: function () {
    return {
      saved_quotes: [],
    };
  },
  created: function () {
    this.indexSavedQuotes();
  },
  methods: {
    indexSavedQuotes: function () {
      axios.get("/saved_quotes").then((response) => {
        console.log("Saved quotes index", response);
        this.saved_quotes = response.data;
      });
    },
  },
};
</script>
