<template>
    <div class="footer-top">
        <div class="container">
            <div class="row">
                <div class="col col-5 text-center" v-for="(item, index) in items" :key="index">
                    <img :src="item.src" alt="">
                    <span>{{item.text}}</span>
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
                    src:'@/assets/img/buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'@/assets/img/buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'@/assets/img/buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'@/assets/img/buy-comics-digital-comics.png',
                    text:'digital comix'
                },
                {
                    src:'@/assets/img/buy-comics-digital-comics.png',
                    text:'digital comix'
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