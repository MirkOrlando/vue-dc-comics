<template>
    <main>
      <div class="container pt-6">
        <div class="row">
          <Comics/>
        </div>
      </div>
      <Banner/>
    </main>
</template>

<script>
import Banner from '@/components/BannerComponent.vue'
import Comics from '@/components/ComicsComponent.vue'

export default {
    name: 'MainComponent',
    components: {
      Banner,
      Comics
    }
}
</script>

<style lang="scss" scoped>

main {
    background: url('@/assets/img/jumbotron.jpg'),linear-gradient(to bottom, $darkerColor, $darkerColor 100%);
    background-size: 100% 30%, cover;
    background-position: top center, bottom;
    background-repeat: no-repeat;
    color: $lightestColor;
    h2 {
      padding: 4rem 0;
    }
}
</style>