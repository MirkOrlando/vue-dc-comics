<template>
  <div id="app">
    <head>
      <link rel="preconnect" href="https://fonts.googleapis.com">
      <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
      <link href="https://fonts.googleapis.com/css2?family=Gudea:wght@400;700&display=swap" rel="stylesheet">
    </head>
    <SiteHeader/>
    <SiteMain/>
    <SiteFooter/>
  </div>
</template>

<script>
import SiteHeader from '@/components/HeaderComponent.vue'
import SiteMain from '@/components/MainComponent.vue'
import SiteFooter from '@/components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<style lang="scss">

@import '@/assets/sass/style.scss';

</style>
