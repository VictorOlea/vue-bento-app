<template>
  <div :class="$style.container">
    <button :class="$style.toggle" @click="toggleDarkMode">
      {{ isDarkMode ? "☀️ Light Mode" : "🌙 Dark Mode" }}
    </button>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from "vue";

const isDarkMode = ref(false);

const toggleDarkMode = () => {
  isDarkMode.value = !isDarkMode.value;
  if (isDarkMode.value) {
    document.documentElement.classList.add("dark");
    localStorage.setItem("theme", "dark");
  } else {
    document.documentElement.classList.remove("dark");
    localStorage.setItem("theme", "light");
  }
};

onMounted(() => {
  const savedTheme = localStorage.getItem("theme");
  if (savedTheme === "dark") {
    isDarkMode.value = true;
    document.documentElement.classList.add("dark");
  }
});
</script>

<style module>
.container {
  position: fixed;
  top: 12px;
  right: 12px;
  z-index: 999; /* Asegura que quede por encima de otros elementos */
}

.toggle {
  background-color: var(--bg-color);
  color: var(--text-color);
  border: none;
  padding: 8px 12px;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.toggle:hover {
  background-color: var(--hover-bg-color);
}
</style>
