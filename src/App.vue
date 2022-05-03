<template>
  <div id="app">
    <SiteHeader/>
    <SiteMain/>
    <footer>Site Footer</footer>
  </div>
</template>

<script>
import SiteHeader from '@/components/HeaderComponent.vue'
import SiteMain from '@/components/MainComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain
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

/* utility */

.h-100 {
  height: 100%;
}

.jc-space-between {
  justify-content: space-between;
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
  padding: 0 1rem;
  margin: 0 1rem;
}

</style>
