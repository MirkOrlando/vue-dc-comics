<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from "@/components/FooterTopComponent.vue";
import FooterBottom from "@/components/FooterBottomComponent.vue";

export default {
  name: "FooterComponent",
  components: {
    FooterTop,
    FooterBottom,
  },
};
</script>