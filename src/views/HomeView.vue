<template>
  <Header />
  <Content />
</template>
<script lang="ts">
import { defineComponent } from "vue";
import Header from "@/components/header.vue";
import Content from "@/components/Content/content.vue";

export default defineComponent({
  components: { Header, Content },
  setup() {
    return {};
  },
});
</script>
