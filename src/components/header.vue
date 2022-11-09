<template>
  <header class="header">
    <nav class="navbar">
      <ul>
        <li>
          <img src="../assets/images/logo.svg" alt="logo" />
        </li>
        <li>
          <Dropdown :title="'Product'" :data="data" />
        </li>
        <li>
          <Dropdown :title="'Company'" :data="data" />
        </li>
        <li>
          <Dropdown :title="'Connect'" :data="data" />
        </li>
      </ul>
      <div class="buttons">
        <button>Login</button>
        <button class="active">Sign Up</button>
      </div>
      <div class="menu_icon">
        <img
          @click="isClosed = false"
          v-if="isClosed"
          src="../assets/images/icon-hamburger.svg"
          alt=""
        />
        <img
          @click="isClosed = true"
          v-else
          src="../assets/images/icon-close.svg"
          alt=""
        />
      </div>
    </nav>
    <div class="header--content">
      <h1>A modren publishing platform</h1>
      <p>Grow your audience and build your online brand</p>
      <div class="btn--wrapper">
        <button>Start for Free</button>
        <button>Learn more</button>
      </div>
    </div>
    <Sidebar v-if="isClosed" />
  </header>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";
import Dropdown from "@/components/resubale/dropdown.vue";
import Sidebar from "@/components/sidebar.vue";

export default defineComponent({
  components: { Dropdown, Sidebar },
  setup() {
    let data = ["Content", "Newsletter", "Linkedin"];

    const isClosed = ref(true);

    return {
      isClosed,
      data,
    };
  },
});
</script>
