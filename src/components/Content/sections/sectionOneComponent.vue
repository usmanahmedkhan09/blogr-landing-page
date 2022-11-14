<template>
  <div class="section--one">
    <h3>Design for the future</h3>
    <div class="description_wrapper">
      <div class="des_content">
        <div class="description">
          <h4>Introducing an extensible editior</h4>
          <p>
            Bloger features an exceedingly intuitive inteface which lets you
            focus on on thing: creating content the editior supports management
            of multiple blogs and allows easy minipulation of embeds such as
            images vedios and marksdowns.Extensibility with plugins and theme
            provide easy ways to add functionality or change the looks of blog
          </p>
        </div>
        <div class="description">
          <h4>Robust content management system</h4>
          <p>
            Flexible content management system enables users to easily mover
            through posts.increase the useability of blogs customized
            categories, section, flow , formates and flow.With this
            functionality, your're in the full control.
          </p>
        </div>
      </div>
      <div class="editior-icon">
        <img
          class="desktop"
          src="../../../assets/images/illustration-editor-desktop.svg"
          alt="desktop"
        />
        <img
          class="mobile"
          src="../../../assets/images/illustration-editor-mobile.svg"
          alt="desktop"
        />
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import editiorIcon from "../../Icons/editior-desktop.vue";

export default defineComponent({
  components: { editiorIcon },
  setup() {
    return {};
  },
});
</script>
