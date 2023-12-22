<script setup>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppShopIcons from './components/AppShopIcons.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppShopIcons />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
