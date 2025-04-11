<template>
  <div :class="$style.grid">
    <slot />
  </div>
</template>

<script setup lang="ts"></script>

<style module>
.grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(6, 100px);
  gap: 12px;
}
</style>
