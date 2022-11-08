<template>
  <footer class="footer">
    <div class="logo_wrapper">
      <img src="../assets/images/logo.svg" alt="logo" />
    </div>
    <div class="list_wrapper">
      <p class="title">Product</p>
      <ul>
        <li>Overview</li>
        <li>Pricing</li>
        <li>MarketPlace</li>
        <li>Features</li>
        <li>Integrations</li>
      </ul>
    </div>
    <div class="list_wrapper">
      <p class="title">Company</p>
      <ul>
        <li>About</li>
        <li>Team</li>
        <li>Blog</li>
        <li>Careers</li>
      </ul>
    </div>
    <div class="list_wrapper">
      <p class="title">Content</p>
      <ul>
        <li>Context</li>
        <li>Newsletter</li>
        <li>linkedin</li>
      </ul>
    </div>
  </footer>
</template>
<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    return {};
  },
});
</script>
