<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><h1>Card-1</h1></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 1 },
      }"
      ><h1>Card-2</h1></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 1 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 1 },
      }"
      ><h1>Card-3</h1></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 4, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><h1>Card-4</h1></BentoCard
    >
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoGrid from "../components/BentoGrid.vue";
import BentoCard from "../components/BentoCard.vue";
</script>

<style module></style>
