<template>
  <h1>local filter ===> username in uppercase : {{ upperCaseFilter }}</h1>
  <h2>username : {{ userName }}</h2>
  <h2>currency in Rs: {{ amount }}</h2>
  <h1>Global filter ===> currency in USD: {{ $filters.currencyUSD(amount) }}</h1>
</template>

<script>
export default {
    data(){
        return{
            userName: "johnny lever",
            amount: 20000,
        };
    },
    computed:{
        upperCaseFilter(){
            return this.userName.toUpperCase();
        },
    },

};
</script>

<style>

</style>