<script lang="ts" setup>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
</script>

<template>
  <main class="app">
    <Header />
    <router-view />
    <Footer />
  </main>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  font:
    normal 1rem 'Leelawadee UI';
  color: var(--primary-font-color);
}

:root {
  --primary-color: rgb(78, 46, 27);
  --primary-font-color: rgb(255, 255, 255);
  --accent-hover: rgb(194, 166, 117);
  --accent-color: rgb(194, 166, 117);
}

.md-18 {
  font-size: 18px;
}

.md-24 {
  font-size: 24px;
}

.md-36 {
  font-size: 36px;
}

.md-48 {
  font-size: 48px;
}

.app {
  min-height: 100vh;
}
</style>
