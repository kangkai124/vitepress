<template>
  <NavBarTitle />

  <div class="flex-grow" />

  <div class="nav">
    <NavBarLinks />
  </div>

  <slot name="search" />
</template>

<script setup lang="ts">
import NavBarTitle from './NavBarTitle.vue'
import NavBarLinks from './NavBarLinks.vue'
</script>

<style scoped>
.flex-grow {
  flex-grow: 1;
}

.nav {
  display: none;
}

@media (min-width: 720px) {
  .nav {
    display: block;
  }
}
</style>
