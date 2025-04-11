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
  width: 100%; /* Ocupa todo el ancho disponible */
  display: flex;
  align-items: center;
  padding-bottom: 0;
  border-bottom: 4px solid var(--border-color, #e0e0e0); /* Usa una variable o valor por defecto */
  margin-bottom: 1rem;
}

.title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 0;
  color: var(--text-color); /* Usa la variable definida en el tema */
  text-align: left;
}
</style>
