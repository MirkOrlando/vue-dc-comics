<template>
  <header>
    <div class="container">
      <div class="row jc-space-between">
        <div class="col">
          <Logo />
        </div>
        <div class="col">
          <NavBarHeader />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import Logo from "@/components/LogoComponent.vue";
import NavBarHeader from "@/components/NavBarComponent.vue";

export default {
  name: "HeaderComponent",
  components: {
    Logo,
    NavBarHeader,
  },
};
</script>

<style lang="scss" scoped>
</style>