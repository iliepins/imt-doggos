<template>
  <div class="layout">
    <header>
      <div class="wrapper">
        <nav>
          <Link
            v-for="navItem in navItems"
            :href="navItem.path"
            :key="navItem.path"
            rel="nofollow"
          >{{ navItem.name }}</Link>
        </nav>
      </div>
    </header>
    <div class="content">
      <slot />
    </div>
  </div>
</template>

<script lang="ts" setup>
import Link from './Link.vue'
import '../assets/main.css'

const navItems = [
  {
    name: 'Home',
    path: import.meta.env.BASE_URL
  },
  {
    name: 'Gallery',
    path: import.meta.env.BASE_URL + `gallery`
  },
  {
    name: 'About finnish dogs',
    path: import.meta.env.BASE_URL + `about-finnish-dogs`
  },
  {
    name: 'Similar breeds',
    path: import.meta.env.BASE_URL + `similar-breeds`
  },
  {
    name: 'Caring tips and mistakes',
    path: import.meta.env.BASE_URL + `care`
  }
]
</script>

<style>
body {
  margin: 0;
  font-family: sans-serif;
}
</style>

<style scoped>
.layout {
  margin: auto;
  max-width: 1280px;
}

.content {
  padding: 20px;
  padding-bottom: 50px;
  min-height: 100vh;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

nav {
  width: 100%;
  padding: 16px 48px;
  font-size: 12px;
  text-align: center;
}



@media (min-width: 1024px) {
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    font-size: 1rem;
  }
}
</style>
