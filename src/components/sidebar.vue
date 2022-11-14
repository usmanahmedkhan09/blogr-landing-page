<template>
  <div class="sidebar">
    <dropdownVue
      class="dark"
      :isLight="false"
      :title="'Product'"
      :data="data"
    />
    <dropdownVue
      class="dark"
      :isLight="false"
      :title="'Company'"
      :data="data"
    />
    <dropdownVue
      class="dark"
      :isLight="false"
      :title="'Connect'"
      :data="data"
    />
    <hr />
    <div class="buttons">
      <button>Login</button>
      <button class="active">Sign Up</button>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import dropdownVue from "./resubale/dropdown.vue";

export default defineComponent({
  components: {
    dropdownVue,
  },
  setup() {
    let data = ["Content", "Newsletter", "Linkedin"];
    return {
      data,
    };
  },
});
</script>
