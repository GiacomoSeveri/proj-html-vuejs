<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain
  }
}
</script>

<template>
  <header>
    <app-header></app-header>
  </header>

  <main>
    <app-main></app-main>
  </main>

  <footer>

  </footer>
</template>

<style lang="scss">
@use './assets/style.scss';
</style>