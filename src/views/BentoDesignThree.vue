<template>
  <BentoGrid>
    <BentoCard :col-span="3" :row-span="3"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-1</h2>
      </section></BentoCard
    >
    <BentoCard :col-span="1" :row-span="4"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-2</h2>
      </section></BentoCard
    >
    <BentoCard :col-span="1" :row-span="3"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-3</h2>
      </section></BentoCard
    >
    <BentoCard :col-span="1" :row-span="3"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-4</h2>
      </section></BentoCard
    >
    <BentoCard :col-span="1" :row-span="3"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Card-5</h2>
      </section></BentoCard
    >
    <BentoCard :col-span="1" :row-span="2"
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
