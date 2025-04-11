<template>
  <footer :class="$style.footer">
    <div :class="$style.container">
      <p>
        &copy; {{ new Date().getFullYear() }} Bento Design Web. Todos los
        derechos reservados.
      </p>
      <nav :class="$style.nav">
        <a href="/terms" :class="$style.link">Términos</a>
        <a href="/privacy" :class="$style.link">Privacidad</a>
        <a href="/contact" :class="$style.link">Contacto</a>
      </nav>
    </div>
  </footer>
</template>

<script setup lang="ts"></script>

<style module>
.footer {
  background: var(--bg-color);
  border: 2px solid var(--border-color, #e0e0e0);
  border-radius: 12px;
  color: var(--text-color);
  padding: 1.5rem;
  text-align: center;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.5rem;
}

.nav {
  display: flex;
  gap: 1rem;
}

.link {
  color: var(--text-color);
  text-decoration: none;
  font-size: 0.875rem;
  transition: color 0.3s ease;
}

.link:hover {
  color: #1abc9c;
}
</style>
