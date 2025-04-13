<template>
  <div class="grid">
    <slot />
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
/* .grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: repeat(6, 100px);
  gap: 12px;
} */

.grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  /* grid-template-rows: repeat(6, 100px); */
  grid-auto-rows: 100px;
  gap: 12px;
}

/* @media (max-width: 1024px) {
  .grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 768px) {
  .grid {
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(4, 100px);
  }
}

@media (max-width: 480px) {
  .grid {
    grid-template-columns: 1fr;
  }
} */
</style>
