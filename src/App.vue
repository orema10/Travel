<template>
  <section class="app">
      <app-header></app-header>
      <app-filter></app-filter>

  </section>
</template>

<script>
import appHeader from './components/Header';
import appFilter from './components/Filter';
export default {
    components: {
      appHeader,
      appFilter
    }
}
</script>


<style>
@import './assets/css/style.css';
</style>
