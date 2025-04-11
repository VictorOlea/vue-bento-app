<template>
  <div :class="$style['section-title']">
    <h2 :class="$style['title']">{{ title }}</h2>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
}>();
</script>

<style module>
.section-title {
  width: 100%;
  display: flex;
  align-items: center;
  padding-bottom: 0;
  border-bottom: 4px solid var(--border-color, #e0e0e0);
  margin-bottom: 1rem;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 0;
  color: var(--text-color);
  text-align: left;
}
</style>
