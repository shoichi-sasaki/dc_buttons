<template>
  <div>
    <button>Default</button>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Button extends Vue {}
</script>

<style scoped>
button {
  width: 81px;
  height: 36px;
  border: none;
  outline: none;
  cursor: pointer;

  background: #e0e0e0;
  box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
  border-radius: 6px;
}
</style>
