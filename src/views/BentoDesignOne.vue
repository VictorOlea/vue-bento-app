<template>
  <BentoGrid>
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 4 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 2 },
      }"
    >
      <div :class="imageStyle['img-wrapper']">
        <img :class="imageStyle['img-card']" src="../assets/rockBand.webp" />
      </div>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 1 },
        tablet: { col: 2, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h1 :class="$style['title-card']">Tigers & Bears</h1>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 4 },
        tablet: { col: 2, row: 3 },
        mobile: { col: 4, row: 3 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Track List</h2>
        <ul :class="sectionStyle['section-content']">
          <li>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</li>
          <li>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</li>
          <li>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</li>
          <li>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</li>
        </ul>
      </section>
    </BentoCard>
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 2 },
        tablet: { col: 2, row: 2 },
        mobile: { col: 4, row: 3 },
      }"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">About Us</h2>
        <p :class="sectionStyle['section-content']">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Non aliquid
          excepturi qui consectetur nostrum quo distinctio delectus eius
          eligendi nobis tenetur ipsum vel, reprehenderit esse fugiat culpa
          modi, enim ex.
        </p>
      </section></BentoCard
    >
    <BentoCard
      :responsive-span="{
        desktop: { col: 2, row: 1 },
        tablet: { col: 4, row: 1 },
        mobile: { col: 4, row: 1 },
      }"
      ><div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/rockBanner.webp"
          alt=""
        /></div
    ></BentoCard>
  </BentoGrid>
</template>

<script setup lang="ts">
import BentoCard from "../components/BentoCard.vue";
import BentoGrid from "../components/BentoGrid.vue";
import imageStyle from "../styles/image.module.css";
import sectionStyle from "../styles/section.module.css";
</script>

<style module>
.img-card {
  width: 100%;
  height: 100%;
  border: 2px solid grey;
  border-radius: 10px;
  object-fit: cover;
}

.title-card {
  font-size: clamp(1.8rem, 4vw, 2.4rem);
  width: 100%;
  height: 100%;
  text-align: center;
  align-self: center;
  padding: 8px;
  margin-top: auto;
  margin-bottom: auto;
}
</style>
