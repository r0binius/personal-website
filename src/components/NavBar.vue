<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <router-link to="/" class="navbar-item">
        <strong>{{ name }}</strong>
      </router-link>
    </div>
    <div class="navbar-menu">
      <div class="navbar-start">
        <router-link to="/" class="navbar-item">Home</router-link>
        <router-link to="/music" class="navbar-item">Music</router-link>
        <router-link to="/projects" class="navbar-item">Projects</router-link>
        <router-link to="/blog" class="navbar-item">Blog</router-link>
      </div>
      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a href="https://codeberg.org/r0binius" target="_blank" class="button is-light">
              <img src="@/assets/icons/git.svg" alt="Codeberg" class="icon" />
            </a>
            <a href="https://open.spotify.com/artist/..." target="_blank" class="button is-light">
              <img src="@/assets/icons/spotify.svg" alt="Spotify" class="icon" />
            </a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup lang="ts">
const name = 'gobin'
</script>

<style scoped>
.navbar {
  background-color: transparent !important;
  padding: 1rem 2rem;
}

.navbar-item {
  color: #9b8ec7 !important;
  font-weight: 500;
}

.navbar-item.router-link-exact-active {
  color: #42b883 !important;
  border-bottom: 2px solid #42b883;
}

.navbar-item:hover {
  color: #42b883 !important;
}

.icon {
  width: 20px;
  height: 20px;
}
</style>
