<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from "./FooterTopComponent.vue";
import FooterBottom from "./FooterBottomComponent.vue";

export default {
  name: "FooterComponent",
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>