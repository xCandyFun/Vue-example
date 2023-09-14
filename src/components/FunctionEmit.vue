<script setup>

const emit = defineEmits(['mySuperCoolEvent'])
const myFunction= () =>{
  console.log("hehh")
  emit("mySuperCoolEvent", "supper sceret")
}
</script>

<template>
  <div>
    FunctionEmit
  <button @click="myFunction">click me</button>
  </div>
</template>

<style scoped>

</style>
