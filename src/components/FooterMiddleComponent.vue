<template>
    <div class="footer-middle">
        <div class="container">
            <div class="row">
                <div class="col col-50 pt-4 pb-4">
                    <div class="row">
                        <div class="col">
                            <div class="row fd-column gy-1">
                                <div class="col m-0 p-0">
                                    <h3>dc comics</h3>
                                    <ul>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                    </ul>
                                </div>
                                <div class="col m-0 p-0">
                                    <h3>shop</h3>
                                    <ul>
                                        <li>lorem</li>
                                        <li>lorem</li>
                                    </ul>
                                </div>
                            </div>                            
                        </div>
                        <div class="col">
                            <h3>dc</h3>
                            <ul>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                            </ul>
                        </div>
                        <div class="col">
                            <h3>sites</h3>
                            <ul>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                                <li>lorem</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col col-50">
                    <div class="logo-lg h-100"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterMiddleComponent',

}
</script>

<style lang="scss" scoped>
@import '@/assets/sass/_variables.scss';

.footer-middle {
    background-image: url('@/assets/img/footer-bg.jpg');
    h3 {
        color: $lightestColor;
        text-transform: uppercase;
    }

    li {
        color: $paleDarkColor;
    }

    .logo-lg {
        background-image: url('@/assets/img/dc-logo-bg.png');
        background-position: center;
        background-repeat: no-repeat;
    }
}
</style>