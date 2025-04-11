<template>
  <BentoGrid>
    <BentoCard :col-span="3" :row-span="3">Card-1</BentoCard>
    <BentoCard :col-span="1" :row-span="4">Card-2</BentoCard>
    <BentoCard :col-span="1" :row-span="3">Card-3</BentoCard>
    <BentoCard :col-span="1" :row-span="3">Card-4</BentoCard>
    <BentoCard :col-span="1" :row-span="3">Card-5</BentoCard>
    <BentoCard :col-span="1" :row-span="2">Card-6</BentoCard>
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoGrid from "../components/BentoGrid.vue";
import BentoCard from "../components/BentoCard.vue";
</script>

<style module></style>
