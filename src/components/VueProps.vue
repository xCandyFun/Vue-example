<script setup>
defineProps({
  showText: {
    type: Boolean,
    required: true
  }
});
</script>

<template>
  <div :class="{myDiv:showText}">
    hej {{showText}}
  </div>
  <h3 v-if="showText">My secret text</h3>
 <h3 v-else>You may not view the secret</h3>
</template>

<style scoped>

.myDiv{
  background-color: chocolate;
}
</style>