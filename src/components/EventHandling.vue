<script setup>
import {ref} from "vue";

const count = ref(0);

function increment(){
  count.value++;
}
</script>

<template>
  <div>
    <button @click="increment">
      Increment
    </button>
    <h2>The Count is:{{ count }}</h2>
  </div>
</template>

<style scoped>
div{
  background-color: tomato;
}
h2 {
  color: blue;
}
</style>