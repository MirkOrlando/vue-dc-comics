<template>
    <header>
      <div class="container">
        <div class="row jc-space-between">
          <div class="col">
            <div class="logo">
              <img src="@/assets/img/dc-logo.png" alt="">
            </div>
          </div>
          <div class="col">
              <NavBarHeader/>
          </div>
        </div>
      </div>
    </header>
</template>

<script>
import NavBarHeader from '@/components/NavBarComponent.vue'

export default {
    name: 'HeaderComponent',
    components: {
        NavBarHeader
    }
}
</script>

<style lang="scss" scoped>
    header {
        .logo {
            display: flex;
            align-items: center;
            height: 100%;
        }
    }
</style>