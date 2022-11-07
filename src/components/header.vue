<template>
  <header class="header">
    <nav class="navbar">
      <ul>
        <li>
          <img src="../assets/images/logo.svg" alt="logo" />
        </li>
        <li>
          <Dropdown :title="'Product'" />
        </li>
        <li>
          <Dropdown :title="'Company'" />
        </li>
        <li>
          <Dropdown :title="'Connect'" />
        </li>
      </ul>
      <div class="buttons">
        <button>Login</button>
        <button class="active">Sign Up</button>
      </div>
    </nav>
  </header>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import Dropdown from "@/components/resubale/dropdown.vue";

export default defineComponent({
  components: { Dropdown },
  setup() {
    return {};
  },
});
</script>
