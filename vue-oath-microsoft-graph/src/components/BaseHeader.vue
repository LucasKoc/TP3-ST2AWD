<script>
import HomePage from "@/pages/HomePage.vue";

export default {
  name: "BaseHeader",
  computed: {
    HomePage() {
      return HomePage
    }
  }
}
</script>

<template>
<div id="header">
  <div class="header-container">
    <div>
        <font-awesome-icon :icon="['fas', 'house']" />
    </div>
    <div>
      <p>Home</p>
    </div>
  </div>

  <div class="header-container">
    <div>
      <p>Not Logged Yet</p>
    </div>
    <div>
      <font-awesome-icon :icon="['fas', 'user']" />
    </div>
  </div>
</div>
</template>

<style scoped>

#header {
  display: flex;
  justify-content: space-between;
  padding: 1em 2em 1em 2em;
  background-color: #42b983;

  height: 3vh;
}

.header-container {
  display: inline-flex;
}

.header-container div {
  display: flex;
  align-items: center;
  margin: 0 0.5em 0 0.5em;
}

</style>