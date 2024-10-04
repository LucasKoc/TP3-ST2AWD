<template>
  <div>
    <base-header />
    <home-page />
    <base-footer />
  </div>
</template>

<script>
import HomePage from './pages/HomePage.vue'
import BaseHeader from "@/components/BaseHeader.vue";
import BaseFooter from "@/components/BaseFooter.vue";

export default {
  name: 'App',
  components: {
    BaseFooter,
    BaseHeader,
    HomePage
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