<template>
  <div class="dropdown" ref="dropdown">
    <div class="d-header">
      <span>{{ title }}</span>
      <arrowLightVue
        v-if="isLight"
        :class="isActive ? 'rotate' : ''"
        @click="isActive = !isActive"
      />
      <arrowDarkVue @click="isActive = !isActive" v-else />
      <!-- <img
        @click="isActive = !isActive"
        src="../../assets/images/icon-arrow-light.svg"
        alt="arrow"
        :class="isActive ? 'rotate' : ''"
      /> -->
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
import arrowLightVue from "../Icons/arrow-light.vue";
import arrowDarkVue from "../Icons/arrow-dark.vue";

export default defineComponent({
  components: { arrowLightVue, arrowDarkVue },
  props: {
    title: {
      type: String,
    },
    data: {
      type: Array,
    },
    isLight: {
      type: Boolean,
      default: true,
    },
  },
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
