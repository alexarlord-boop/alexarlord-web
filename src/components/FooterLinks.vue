<template>
  <div id="links">
   <slot></slot>
  </div>
</template>

<script>
import FooterLink from "@/components/FooterLink.vue";

export default {
  name: "FooterLinks",
  components: {FooterLink}
}
</script>

<style lang="sass">


</style>