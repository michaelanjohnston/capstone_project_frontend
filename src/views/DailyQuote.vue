<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div>
      <p>Quote: {{ dailyquote }}</p>
    </div>
  </div>
</template>

<style></style>

<script>
import axios from "axios";
export default {
  data: function () {
    return {
      dailyquote: "Here is a quote!",
    };
  },
  created: function () {
    this.indexDailyQuote;
  },
  methods: {
    DailyQuote: function () {
      axios.get("http://localhost:3000/dailyquote").then((response) => {
        console.log("Daily Inspirational Quote", response.data);
        this.dailyquote = response.data;
      });
    },
  },
};
</script>
