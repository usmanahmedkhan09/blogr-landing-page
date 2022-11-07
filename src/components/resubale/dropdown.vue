<template>
  <div class="dropdown" ref="dropdown">
    <div class="d-header">
      <span>{{ title }}</span>
      <img
        @click="isActive = !isActive"
        src="../../assets/images/icon-arrow-light.svg"
        alt="arrow"
        :class="isActive ? 'rotate' : ''"
      />
    </div>
    <div class="content" :class="isActive ? 'active' : ''">
      <div class="data" v-for="(item, index) in data" :key="index">
        {{ item }}
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import { onClickOutside } from "@vueuse/core";

export default defineComponent({
  props: ["title", "data"],
  setup() {
    const dropdown = ref(null);

    const isActive = ref(false);

    const close = () => {
      isActive.value = false;
    };

    onClickOutside(dropdown, close);

    return { isActive, dropdown };
  },
});
</script>
