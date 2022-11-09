<template>
  <Header />
  <!-- <Content />
  <Footer /> -->
</template>
<script lang="ts">
import { defineComponent } from "vue";
import Header from "@/components/header.vue";
import Content from "@/components/Content/content.vue";
import Footer from "@/components/footer.vue";

export default defineComponent({
  components: { Header, Content, Footer },
  setup() {
    return {};
  },
});
</script>
