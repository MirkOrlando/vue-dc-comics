<template>
    <main>
      <div class="container">
        <h2>** Content goes here **</h2>
      </div>
    </main>
</template>

<script>
export default {
    name: 'MainComponent'
}
</script>

<style lang="scss" scoped>
@import '@/assets/sass/_variables.scss';

main {
    background-color: $darkerColor;
    color: $lightestColor;
    padding: 4rem;
}
</style>