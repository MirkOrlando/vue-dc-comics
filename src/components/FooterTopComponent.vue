<template>
    <div class="footer-top">
        <div class="container">
            <div class="row">
                <div class="col col-5 text-center" v-for="(item, index) in items" :key="index">
                    <img :src="'@/assets/img/' + item.src" alt="">
                    <div>{{item.text}}</div>
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
                    src:'buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'buy-comics-merchandise.png',
                    text:'dc merchandise'
                },
                {
                    src:'buy-comics-subscriptions.png',
                    text:'subscription'
                },
                {
                    src:'buy-comics-shop-locator.png',
                    text:'comic shop lacator'
                },
                {
                    src:'buy-dc-pover-visa.png',
                    text:'dc power visa'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.footer-top {
    background-color: cornflowerblue;
    color: white;
}
</style>