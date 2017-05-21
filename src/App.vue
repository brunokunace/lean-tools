<template>
  <!-- Don't drop "q-app" class -->
  <q-layout id="q-app">
      <app-header></app-header>
      <router-view class="layout-view"></router-view>
  </q-layout>
</template>

<script>
import Header from './components/Header.vue'

export default {
  components: {
    appHeader: Header
  }
}
</script>

<style>

</style>
