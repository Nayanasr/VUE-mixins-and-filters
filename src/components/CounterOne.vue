<template>
  <h1> COUNTER ONE :{{ counter }}</h1>
  <button @click="increment"> Increment </button>
  <button @click="decrement">Decrement</button>
  <button @click="reset">Reset</button>
</template>

<script>
import counterMixins from '@/mixins/CounterMixins'
export default {
   mixins:[counterMixins(0,10)]


}
</script>

<style>

</style>