<template>
  <div class="dropdown">
    <div class="wrapper">
      <span>{{ title }}</span>
      <img src="../../assets/images/icon-arrow-light.svg" alt="arrow" />
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: ["title"],
  setup() {
    return {};
  },
});
</script>
