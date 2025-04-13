<template>
  <BentoGrid :class="$style['bento-grid']">
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
    >
      <section :class="sectionStyle['section-card']">
        <h1 :class="$style['title-card']">日本へようこそ！</h1>
      </section>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h1 :class="$style['title-card']">Ichi-go ichi-e (一期一会)</h1>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 4, row: 4 },
        mobile: { col: 4, row: 2 },
      }"
      ><div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/japanCityMountain.jpg"
          alt="Vista de la montaña en la ciudad de Japón"
        /></div
    ></BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Disfruta</h2>
        <p :class="sectionStyle['section-content']">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit.
        </p>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 5 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><div :class="imageStyle['img-wrapper']">
        <img
          src="../assets/japanCityNight.jpg"
          alt="Vista de la ciudad de Japón"
          :class="imageStyle['img-card']"
        /></div
    ></BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/japanCity.jpg"
          alt="Noche en la ciudad de Japón"
        /></div
    ></BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 1, row: 3 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Explora Japón</h2>
        <p :class="sectionStyle['section-content']">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Assumenda
          quasi voluptate voluptas? Similique quae quis ex hic sint velit
          asperiores dolorem porro quaerat. Velit, est! Laborum reiciendis
          corporis sit nobis!
        </p>
      </section></BentoCard
    >
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoCard from "../components/BentoCard.vue";
import BentoGrid from "../components/BentoGrid.vue";
import imageStyle from "../styles/image.module.css";
import sectionStyle from "../styles/section.module.css";
</script>

<style module>
.title-card {
  font-size: 1.8em;
  overflow: hidden;
  height: 100%;
  width: 100%;
}
</style>
