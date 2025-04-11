<template>
  <BentoGrid>
    <BentoCard :colSpan="2" :rowSpan="4">
      <div :class="imageStyle['img-wrapper']">
        <img :class="imageStyle['img-card']" src="../assets/rockBand.jpg" />
      </div>
    </BentoCard>
    <BentoCard :colSpan="2" :rowSpan="1"
      ><section :class="sectionStyle['section-card']">
        <h1 :class="$style['title-card']">Lions, Tigers & Bears</h1>
      </section></BentoCard
    >
    <BentoCard :colSpan="2" :rowSpan="4"
      ><section :class="sectionStyle['section-card']">
        <h2 :class="sectionStyle['section-title']">Track List</h2>
        <p :class="sectionStyle['section-content']">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit.
        </p>
        <p :class="sectionStyle['section-content']">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit.
        </p>
        <p :class="sectionStyle['section-content']">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit.
        </p>
      </section>
    </BentoCard>
    <BentoCard :colSpan="2" :rowSpan="2"
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
    <BentoCard :colSpan="2" :rowSpan="1"
      ><div :class="imageStyle['img-wrapper']">
        <img
          :class="imageStyle['img-card']"
          src="../assets/rockBanner.jpg"
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
  font-size: 1.8em;
  overflow: hidden;
  height: 100%;
  width: 100%;
}
</style>
