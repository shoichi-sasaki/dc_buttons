<template>
  <div id="display">
    <div class="sub-title">Buttons</div>
    <div class="buttons-box">
      <Button variant="huaghuga" disableShadow/>
      <!-- <div v-for="item in items" :key="item" class="contents">{{ item }}</div> -->
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Button from "./Button.vue";

@Component({
  components: {
    Button
  }
})
export default class Buttons extends Vue {}
</script>

<style scoped>
#display {
  position: absolute;
  left: 320px;
  top: 53px;
}
.sub-title {
  font-family: Poppins;
  font-style: normal;
  font-weight: 500;
  font-size: 24px;
  line-height: 36px;

  color: #4f4f4f;
}
</style>
