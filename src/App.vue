<template>
  <div id="app">
    <Sidebar />
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <Buttons />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Sidebar from "./components/Sidebar.vue";
import Buttons from "./components/Buttons.vue";

@Component({
  components: {
    Sidebar,
    Buttons
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
