<template>
  <main class="content">
    <SectionOne />
    <SectionTwo />
    <sectionThree />
  </main>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import SectionOne from "@/components/Content/sections/sectionOneComponent.vue";
import SectionTwo from "@/components/Content/sections/sectionTwoComponent.vue";
import sectionThree from "@/components/Content/sections/sectionThreeComponent.vue";

export default defineComponent({
  components: { SectionOne, SectionTwo, sectionThree },
  setup() {
    return {};
  },
});
</script>
