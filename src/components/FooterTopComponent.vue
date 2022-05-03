<template>
    <div class="footer-top">
        <div class="container">
            <div class="row pt-4 pb-4">
                <div class="col col-5 text-center" v-for="(item, index) in items" :key="index">
                    <div class="wrapper">
                        <img :src="require(`@/assets${item.src}`)" alt="">
                        <div class="text">{{item.text}}</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterTopComponent',
    data() {
        return{
            items:[
                {
                    src:'/img/buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'/img/buy-comics-merchandise.png',
                    text:'dc merchandise'
                },
                {
                    src:'/img/buy-comics-subscriptions.png',
                    text:'subscription'
                },
                {
                    src:'/img/buy-comics-shop-locator.png',
                    text:'comic shop lacator'
                },
                {
                    src:'/img/buy-dc-power-visa.svg',
                    text:'dc power visa'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/sass/_variables.scss';

.footer-top {
    background-color: $primaryColor;
    color: $lightestColor;

    .wrapper {
        display: flex;
        align-items: center;
        gap: 0.5rem;

        img {
            height: 50px;
        }

        .text {
            text-transform: uppercase;
        }

    }
}
</style>