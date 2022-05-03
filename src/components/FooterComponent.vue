<template>
    <footer>
        <FooterTop/>
        <FooterMiddle/>
      <div class="footer-bottom">footer-bottom</div>
    </footer>
</template>

<script>
import FooterTop from '@/components/FooterTopComponent.vue'
import FooterMiddle from '@/components/FooterMiddleComponent.vue'

export default {
    name: 'FooterComponent',
    components: {
        FooterTop,
        FooterMiddle
    }
}
</script>