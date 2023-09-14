<script setup>
import {computed, ref} from "vue";

const  counter = ref(0);

const doubleCounter = computed(()=>counter.value*2);
</script>

<template>
  <div @click="counter++">it can count: {{counter}}</div>
  <p> doublecounter {{doubleCounter}}</p>
</template>

<style scoped>

</style>
