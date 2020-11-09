<template>
  <div id="sidebar">
    <div class="title"><span class="title-colored">Dev</span>challenges.io</div>
    <div class="contents-box">
      <div v-for="item in items" :key="item" class="contents">{{ item }}</div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
  // public items:
  private items: Array<string> = [
    "Colors",
    "Typography",
    "Spaces",
    "Buttons",
    "Inputs",
    "Grid"
  ];
  private greet = "Hello";

  private onGreet() {
    alert(this.greet);
    this.greet = "こんにちは";
  }
}
</script>

<style scoped>
#sidebar {
  position: absolute;
  width: 237px;
  /* height: 1234px; */
  height: 100vh;
  top: 0px;
  left: 0px;

  background: #fafbfd;
}
.title {
  position: absolute;
  width: 114px;
  height: 20px;
  left: 48px;
  top: 38px;

  font-family: Poppins;
  font-style: normal;
  font-weight: 600;
  font-size: 13px;
  line-height: 19px;
  /* identical to box height */
}
.title-colored {
  color: #f7542e;
}
.contents-box {
  position: absolute;
  width: 62px;
  /* height: 20px; */
  left: 48px;
  top: 180px;

  font-family: Noto Sans JP;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 20px;

  color: #9e9e9e;
}
.contents {
  padding-bottom: 25px;
  text-align: left;
}
</style>
