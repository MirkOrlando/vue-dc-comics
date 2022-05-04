<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="row jc-space-between ai-center pb-2 pt-2">
                <div class="col">
                    <a href="#" class="btn-primary-outline">Sign-up now!</a>
                </div>
                <div class="col">
                    <div class="social">
                        <div class="text">follow us</div>
                        <div class="social-icons">
                            <img src="@/assets/img/footer-facebook.png" alt="">
                            <img src="@/assets/img/footer-twitter.png" alt="">
                            <img src="@/assets/img/footer-youtube.png" alt="">
                            <img src="@/assets/img/footer-pinterest.png" alt="">
                            <img src="@/assets/img/footer-periscope.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterBottomComponent',

}
</script>

<style lang="scss" scoped>

.footer-bottom {
    background-color: $darkColor;

    .social {
        display: flex;
        align-items: center;
        gap: 1rem;

        .text {
            text-transform: uppercase;
            color: $primaryColor;
            font-weight: bold;
        }

        img {
            margin-left: 1rem;
            transition: all 250ms linear;
            &:hover {
                cursor: pointer;
                transform: scale(0.90);
            }
        }
    }
}
</style>