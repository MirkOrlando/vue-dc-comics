<template>
    <main>
      <div class="container">
        <h2>** Content goes here **</h2>
      </div>
      <Banner/>
    </main>
</template>

<script>
import Banner from '@/components/BannerComponent.vue'

export default {
    name: 'MainComponent',
    components: {
      Banner
    }
}
</script>

<style lang="scss" scoped>

main {
    background-color: $darkerColor;
    color: $lightestColor;
    h2 {
      padding: 4rem 0;
    }
}
</style>