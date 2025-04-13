<!-- <template>
  <div
    :class="$style.card"
    :style="{
      gridColumn: `span ${colSpan}`,
      gridRow: `span ${rowSpan}`,
    }"
  >
    <slot />
  </div>
</template> -->

<template>
  <div
    :class="$style.card"
    :style="{
      gridColumn: `span ${currentSpan.col}`,
      gridRow: `span ${currentSpan.row}`,
    }"
  >
    <slot />
  </div>
</template>

<script setup lang="ts">
import { computed, ref, onMounted, onUnmounted } from "vue";

const props = defineProps<{
  responsiveSpan: {
    desktop: { col: number; row: number };
    tablet?: { col: number; row: number };
    mobile?: { col: number; row: number };
  };
}>();

const screenWidth = ref(window.innerWidth);

const updateWidth = () => {
  screenWidth.value = window.innerWidth;
};

onMounted(() => window.addEventListener("resize", updateWidth));
onUnmounted(() => window.removeEventListener("resize", updateWidth));

const currentSpan = computed(() => {
  if (screenWidth.value <= 480 && props.responsiveSpan.mobile) {
    return props.responsiveSpan.mobile;
  } else if (screenWidth.value <= 768 && props.responsiveSpan.tablet) {
    return props.responsiveSpan.tablet;
  }
  return props.responsiveSpan.desktop;
});

// defineProps({
//   colSpan: {
//     type: Number,
//     default: 1,
//   },
//   rowSpan: {
//     type: Number,
//     default: 1,
//   },
// });
</script>

<style module>
.card {
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  background-color: #f3f4f6;
  color: #000000;
  padding: 8px;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-4px);
}
</style>
