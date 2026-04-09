<script setup lang="ts">
const name = 'gobin'
const tagline = 'music production · art · development'
</script>

<template>
  <main class="container">
    <h1 class="title">{{ name }}</h1>
    <p class="tagline">{{ tagline }}</p>

    <nav class="links">
      <a href="/about">About</a>
      <a href="/music">Music</a>
      <a href="/projects">Projects</a>
      <a href="/blog">Blog</a>
    </nav>

    <div class="social-links">
      <a
        href="https://codeberg.org/r0binius"
        target="_blank"
        title="Codeberg"
        aria-label="Codeberg"
      >
        <img src="@/assets/icons/git.svg" alt="Codeberg" class="social-icon" />
      </a>
      <a
        href="https://open.spotify.com/artist/..."
        target="_blank"
        title="Spotify"
        aria-label="Spotify"
      >
        <img src="@/assets/icons/spotify.svg" alt="Spotify" class="social-icon" />
      </a>
      <a
        href="https://soundcloud.com/..."
        target="_blank"
        title="SoundCloud"
        aria-label="SoundCloud"
      >
        <img src="@/assets/icons/soundcloud.svg" alt="SoundCloud" class="social-icon" />
      </a>
    </div>
  </main>
</template>

<style scoped>
@import url('assets/css/fonts.css');

.container {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 16px;
  font-family:
    'Velvetine',
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

.links,
.social-links {
  display: flex;
  gap: 20px;
  margin-top: 20px;
}

.links a,
.social-links a {
  text-decoration: none;
  font-weight: 500;
  color: #9b8ec7;
}

.links a:hover,
.social-links a:hover {
  text-decoration: underline;
}

.social-links {
  margin-top: 30px;
}

.social-icon {
  width: 24px;
  height: 24px;
  transition: color 0.3s;
  color: #bda6ce;
}

.social-links a:hover .social-icon {
  color: #bda6ce;
}
</style>
