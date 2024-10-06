<script>
import BaseButton from "@/components/BaseButton.vue";

export default {
  name: "HomePage",
  components: {
    BaseButton,
  },
}
</script>

<template>
  <div class="main">
    <div>
      <p>Here is the content of the HomePage</p>
    </div>

    <div>
      <base-button role="button" color="primary">BaseButton</base-button>
      <base-button role="button" :disabled="true">BaseButton Disabled</base-button>
      <base-button role="button" color="warn">BaseButton with color props</base-button>
      <base-button role="button" color="danger">BaseButton with color props</base-button>
    </div>
  </div>
</template>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
}

div.main {
  display: flex;
  flex-direction: column;
  align-items: center;
}

div {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>