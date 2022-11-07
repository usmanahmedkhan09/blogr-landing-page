<template>
  <main class="content">
    <SectionOne />
  </main>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import SectionOne from "./sections/sectionOneComponenet.vue";

export default defineComponent({
  components: { SectionOne },
  setup() {
    return {};
  },
});
</script>
