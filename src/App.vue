<script setup>
import LoopDirective from "@/components/LoopDirective.vue";
import EventHandling from "./components/EventHandling.vue"
import VueProps from "./components/VueProps.vue"
import SlotContainer from "@/components/SlotContainer.vue";
</script>

<template>
  <SlotContainer>
  <h1>Hej detta är test</h1>
  <EventHandling />
  <LoopDirective />
  <VueProps :showText="true" />
  <VueProps :showText="false" />
  </SlotContainer>
</template>

<style scoped>
h1{
  width: 100%;
  text-align: center;
}
</style>
