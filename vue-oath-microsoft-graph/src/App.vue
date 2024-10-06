<template>
  <div>
    <base-layout>
      <home-page />
    </base-layout>
  </div>
</template>

<script>
import HomePage from './pages/HomePage.vue'
import BaseLayout from './layouts/BaseLayout.vue'

export default {
  name: 'App',
  components: {
    HomePage,
    BaseLayout
  }
}
</script>

<style>
* {
  font-family: 'Montserrat', 'Arial', sans-serif;
}

body {
  margin: 0;

  min-height: 100%;
}
</style>