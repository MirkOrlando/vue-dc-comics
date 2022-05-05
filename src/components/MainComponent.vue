<template>
  <main>
    <Hero />
    <Comics />
    <Banner />
  </main>
</template>

<script>
import Hero from "@/components/HeroComponent.vue";
import Comics from "@/components/ComicsSectionComponent.vue";
import Banner from "@/components/BannerComponent.vue";

export default {
  name: "MainComponent",
  components: {
    Hero,
    Comics,
    Banner,
  },
};
</script>

<style lang="scss" scoped>
</style>