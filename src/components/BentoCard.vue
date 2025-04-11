<template>
  <div
    :class="$style.card"
    :style="{
      gridColumn: `span ${colSpan}`,
      gridRow: `span ${rowSpan}`,
    }"
  >
    <slot />
  </div>
</template>

<script setup lang="ts">
defineProps({
  colSpan: {
    type: Number,
    default: 1,
  },
  rowSpan: {
    type: Number,
    default: 1,
  },
});
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
