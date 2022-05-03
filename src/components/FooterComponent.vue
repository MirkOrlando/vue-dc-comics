<template>
    <footer>
        <FooterTop/>
      <div class="footer-middle">footer-middle</div>
      <div class="footer-bottom">footer-bottom</div>
    </footer>
</template>

<script>
import FooterTop from '@/components/FooterTopComponent.vue'

export default {
    name: 'FooterComponent',
    components: {
        FooterTop
    }
}
</script>