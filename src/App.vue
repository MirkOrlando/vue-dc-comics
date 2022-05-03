<template>
  <div id="app">
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

/* common */

body {
  overflow-x: hidden;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

ul {
  list-style: none;
}

/* utility */

.h-100 {
  height: 100%;
}

.pt-4 {
  padding-top: 4rem;
}

.pb-4 {
  padding-bottom: 4rem;
}

.jc-space-between {
  justify-content: space-between;
}

.fd-column {
  flex-direction: column;
}

.gy-1 {
  row-gap: 1rem;
}

.text-center {
  text-align: center;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* grid structure */

.container {
  max-width: 1440px;
  margin: auto;
}

.row {
  display: flex;
  margin: 0 -1rem;
}

.col {
  padding-left: 1rem;
  padding-right: 1rem;
  margin: 0 1rem;
}

.col-5 {
  width: calc(100%/12)*5;
}

.col-50 {
  width: 50%;
}

</style>
