<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 3, row: 3 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-1</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 4 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-2</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 4, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-3</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 4, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-4</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-5</h2>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-6</h2>
      </section></BentoCard
    >
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoGrid from "../components/BentoGrid.vue";
import BentoCard from "../components/BentoCard.vue";
import sectionStyle from "../styles/section.module.css";
</script>

<style module></style>
