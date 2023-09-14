<script setup>
import LoopDirective from "@/components/LoopDirective.vue";
import EventHandling from "./components/EventHandling.vue"
import VueProps from "./components/VueProps.vue"
import SlotContainer from "@/components/SlotContainer.vue";
import ComputedVariable from "@/components/ComputedVariable.vue";
import SimpelEmit from "@/components/simpelEmit.vue";
import FunctionEmit from "@/components/FunctionEmit.vue";

const HandleEvent = (SV) =>{
  console.log('Handling', SV)
}
</script>

<template>
  <SlotContainer>
    <h1>Hej detta är test</h1>
    <EventHandling/>
    <LoopDirective/>
    <VueProps :showText="true"/>
    <VueProps :showText="false"/>
    <ComputedVariable/>
    <SimpelEmit @my-emit-event="(number) => console.log('Caught custom event', number)"/>
    <FunctionEmit @my-super-cool-event="HandleEvent" />
  </SlotContainer>
</template>

<style scoped>
h1 {
  width: 100%;
  text-align: center;
}
</style>
