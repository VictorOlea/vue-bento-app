<script setup lang="ts">
import DarkModeToggle from "./components/DarkModeToggle.vue";
import Header from "./components/Header.vue";
import BentoDesignOne from "./views/BentoDesignOne.vue";
import BentoDesignTwo from "./views/BentoDesignTwo.vue";
import BentoDesignThree from "./views/BentoDesignThree.vue";
import SectionTitle from "./components/SectionTitle.vue";
import Footer from "./components/PageFooter.vue";
</script>

<template>
  <DarkModeToggle />
  <Header title="Bento Vue App" subtitle="A simple app with Vue 3" />
  <SectionTitle title="Bento Example-1" />
  <bento-design-one />
  <br />
  <SectionTitle title="Bento Example-2" />
  <bento-design-two />
  <br />
  <SectionTitle title="Bento Example-3" />
  <bento-design-three />
  <br />
  <Footer />
</template>
