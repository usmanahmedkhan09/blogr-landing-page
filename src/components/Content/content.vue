<template>
  <main class="content">
    <SectionOne />
    <SectionTwo />
  </main>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import SectionOne from "@/components/Content/sections/sectionOneComponent.vue";
import SectionTwo from "@/components/Content/sections/sectionTwoComponent.vue";

export default defineComponent({
  components: { SectionOne, SectionTwo },
  setup() {
    return {};
  },
});
</script>
