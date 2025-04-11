<template>
  <header :class="$style['header']">
    <h1 :class="$style['title']">{{ title }}</h1>
    <p :class="$style['subtitle']">{{ subtitle }}</p>
  </header>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
  subtitle: string;
}>();
</script>

<style module src="../styles/header.module.css"></style>
