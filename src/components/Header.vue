<script lang="ts" setup>
import { RouterLink } from 'vue-router'
import { RouteDefs, routes } from '@/config/navigation.ts'
</script>

<template>
  <header>
    <RouterLink :to="RouteDefs.Home" class="logo">
      <div class="icon-logo">
        <img alt="Logo" src="/favicon.png" />
      </div>
      <p>Cachacaria Wilbert</p>
    </RouterLink>

    <div class="items">
      <RouterLink
        v-for="item in routes"
        :key="item.path"
        :to="item.path"
        active-class="active"
        class="item"
      >
        {{ item.name }}
      </RouterLink>
    </div>
  </header>
</template>

<style scoped>
header {
  background: var(--primary-color);
  padding: 6px;
  padding-left: 20px;
  padding-right: 20px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

header p {
  color: #fff;
  font-size: 1.2rem;
}

.icon-logo img {
  width: 100px;
}

.logo {
  display: flex;
  align-items: center;
  cursor: pointer;
}

.logo p {
  cursor: pointer;
  transition:
    color 0.25s,
    font-size 0.25s;
}

.logo p:hover {
  color: var(--accent-hover);
  font-size: calc(100% + 4px);
}

.icon-logo {
  transition: scale 0.25s;
}

.icon-logo:hover {
  scale: 1.1;
}

.items {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 32px;
}

.item {
  color: #fff;
  cursor: pointer;
  transition:
    color 0.25s,
    font-size 0.25s;
}

.item:hover,
.item.active {
  color: var(--accent-hover);
  font-size: calc(100% + 2px);
}
</style>
