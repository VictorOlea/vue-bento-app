<template>
  <header :class="$style['header']">
    <div :class="$style['container']">
      <h1 :class="$style['title']">{{ title }}</h1>
      <p :class="$style['subtitle']">{{ subtitle }}</p>
    </div>
  </header>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
  subtitle: string;
}>();
</script>

<style module src="../styles/header.module.css"></style>
