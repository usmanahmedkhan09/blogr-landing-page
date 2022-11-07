<template>
  <header class="header">
    <nav class="navbar">
      <ul>
        <li>
          <img src="../assets/images/logo.svg" alt="logo" />
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
// import Helpers from "@/helpers/helpers";

export default defineComponent({
  setup() {
    // const getImage = (url: string) => Helpers.getImageUrl(url);
    return {
      // getImage,
    };
  },
});
</script>
