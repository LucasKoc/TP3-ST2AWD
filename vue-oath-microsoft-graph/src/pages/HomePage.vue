<script>
import BaseButton from "@/components/BaseButton.vue";
import AsyncButton from "@/components/AsyncButton.vue";

export default {
  name: "HomePage",
  components: {
    AsyncButton,
    BaseButton,
  },

  methods: {
    handleAsyncClick() {
      return new Promise((resolve) => {
        setTimeout(() => {
          resolve();
        }, 2000);
      });
    },
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

      <async-button color="primary" @click="handleAsyncClick">Click Me (Disabled for 1s/click)</async-button>
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