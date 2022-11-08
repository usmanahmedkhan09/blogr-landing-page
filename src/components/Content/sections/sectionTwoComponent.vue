<template>
  <div class="section--two">
    <div class="icons_wrapper">
      <img
        src="../../../assets/images/illustration-phones.svg"
        alt=""
        srcset=""
      />
      <!-- <PhonesIcon /> -->
    </div>
    <div class="description_wrapper">
      <h3>State of the Art infrastructure</h3>
      <p>
        With reliabilitiy and speed in mind, worldwide data centers provide the
        backbone for ultra fast connectivity.This ensures your site will load
        instantly, no matters where your reader are, keeping your site
        competitive.
      </p>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import PhonesIcon from "../../Icons/phones.vue";

export default defineComponent({
  components: { PhonesIcon },
  setup() {
    return {};
  },
});
</script>
