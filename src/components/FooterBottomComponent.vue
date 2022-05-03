<template>
    <div class="footer-bottom">
        <div class="container">
            <div class="row jc-space-between ai-center pb-2 pt-2">
                <div class="col">
                    <a href="#" class="btn">Sign-up now!</a>
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
    background-color: #383838;
    .btn {
        display: inline-block;
        text-decoration: none;
        color: white;
        border: 4px solid cornflowerblue;
        padding: 0.5rem;
        text-transform: uppercase;
    }

    .social {
        display: flex;
        align-items: center;
        gap: 1rem;

        .text {
            text-transform: uppercase;
            color: cornflowerblue;
            font-weight: bold;
        }

        img {
            margin-left: 1rem;
        }
    }
}
</style>