<script setup lang="ts">
const name = 'gobin'
const tagline = 'Music Producer · Developer'
</script>

<template>
  <main class="container">
    <h1 class="title">{{ name }}</h1>
    <p class="tagline">{{ tagline }}</p>

    <nav class="links">
      <a href="/music">Music</a>
      <a href="/projects">Projects</a>
      <a href="https://github.com/r0binius" target="_blank">GitHub</a>
    </nav>
  </main>
</template>

<style scoped>
.container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 16px;

  font-family:
    system-ui,
    -apple-system,
    sans-serif;
  text-align: center;
}

.title {
  font-size: 3rem;
  font-weight: 700;
  margin: 0;
}

.tagline {
  font-size: 1.2rem;
  opacity: 0.7;
}

.links {
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

.links a {
  text-decoration: none;
  font-weight: 500;
  color: #42b883;
}

.links a:hover {
  text-decoration: underline;
}
</style>
