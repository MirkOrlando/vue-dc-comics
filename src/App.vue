<template>
  <div id="app">
    <SiteHeader/>
    <main>Site Main</main>
    <footer>Site Footer</footer>
  </div>
</template>

<script>
import SiteHeader from '@/components/HeaderComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHeader
  }
}
</script>

<style lang="scss">

/* common */

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

.col-40 {
  width: 40%;
}

.col-60 {
  width: 60%;
}

</style>
