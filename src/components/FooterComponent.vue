<template>
    <footer>
        <FooterTop/>
        <FooterMiddle/>
        <FooterBottom/>
    </footer>
</template>

<script>
import FooterTop from '@/components/FooterTopComponent.vue'
import FooterMiddle from '@/components/FooterMiddleComponent.vue'
import FooterBottom from '@/components/FooterBottomComponent.vue'

export default {
    name: 'FooterComponent',
    components: {
        FooterTop,
        FooterMiddle,
        FooterBottom
    }
}
</script>