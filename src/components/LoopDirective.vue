<script setup>

import {ref} from "vue";

const frukter = ref(["apelsin","äpple","bannan"]);

const filterArray = (frukt) =>{
  frukter.value = frukter.value.filter((removeFruit) => removeFruit !== frukt)
}
</script>

<template>
  <div>
    <ol>
      <li v-for="frukt in frukter" :key="frukt">
        {{frukt}}
        <button @click="filterArray(frukt)">
          Remove
        </button>
      </li>
    </ol>
  </div>
</template>

<style scoped>
div{
  background-color: aqua;
}
</style>