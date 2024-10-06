<script>
export default {
  name: "BaseButton",
  props: {
    disabled: {
      type: Boolean,
      default: false,
    },
  },
  methods: {
    handleClick(event) {
      if (this.disabled) {
        event.preventDefault();
      }
    },
  },
};
</script>

<template>
  <button
      v-bind="$attrs"
      :disabled="disabled"
      :class="{ 'disabled': disabled }"
      @click="handleClick">
    <slot></slot>
  </button>
</template>

<style scoped>
button {
  margin: 0.5em;
  padding: 10px 20px;
  background-color: #42b983;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.3s ease;
}

button:hover:not(.disabled),
button:focus:not(.disabled) {
  background-color: #36876d;
  transform: scale(1.10);
}

button.disabled {
  background-color: #42b983;
  cursor: not-allowed;
  opacity: 0.6;
}
</style>