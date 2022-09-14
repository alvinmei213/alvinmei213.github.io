<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template lang="pug">
header
  .wrapper
    nav
      RouterLink(to="/") Home
      RouterLink(to="/about") About
RouterView
</template>

<style scoped>

</style>
