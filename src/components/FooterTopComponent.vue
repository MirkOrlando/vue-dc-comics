<template>
    <div class="footer-top">
        <div class="container">
            <div class="row jc-space-between">
                <div class="col col-50 pt-4 pb-4">
                    <LinksList/>
                </div>
                <div class="col col-50">
                    <div class="logo-lg h-100"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import LinksList from '@/components/LinksListComponent.vue'

export default {
    name: 'FooterTopComponent',
    components: {
        LinksList
    }

}
</script>

<style lang="scss" scoped>

.footer-top {
    background-image: url('@/assets/img/footer-bg.jpg');

    .logo-lg {
        background-image: url('@/assets/img/dc-logo-bg.png');
        background-position: center;
        background-repeat: no-repeat;
    }
}
</style>