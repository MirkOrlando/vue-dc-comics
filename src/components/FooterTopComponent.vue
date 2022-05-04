<template>
    <div class="footer-top">
        <div class="container">
            <div class="row jc-space-between">
                <div class="col col-50 pt-4 pb-4">
                    <div class="row fw-wrap">
                        <FooterMenu :title="title" :links="links" v-for="({title, links}, index) in footerMenu" :key="index"/>
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
import FooterMenu from '@/components/FooterMenuComponent.vue'

export default {
    name: 'FooterTopComponent',
    components: {
        FooterMenu
    },
    data() {
        return {
            footerMenu: [
                {
                    title: 'DC Comics',
                    links: [
                        {
                            href: '#',
                            text: 'Characters'
                        },
                        {
                            href: '#',
                            text: 'Comics'
                        },
                        {
                            href: '#',
                            text: 'Movies'
                        },
                        {
                            href: '#',
                            text: 'TV'
                        },
                        {
                            href: '#',
                            text: 'Games'
                        },
                        {
                            href: '#',
                            text: 'Videos'
                        },
                        {
                            href: '#',
                            text: 'News'
                        },
                    ]
                },
                {
                    title: 'DC',
                    links: [
                        {
                            href: '#',
                            text: 'Terms of Use'
                        },
                        {
                            href: '#',
                            text: 'Privacy Policy (New)'
                        },
                        {
                            href: '#',
                            text: 'Ad Choises'
                        },
                        {
                            href: '#',
                            text: 'Advertising'
                        },
                        {
                            href: '#',
                            text: 'Jobs'
                        },
                        {
                            href: '#',
                            text: 'Subscription'
                        },
                        {
                            href: '#',
                            text: 'Talent Workshop'
                        },
                        {
                            href: '#',
                            text: 'CPSC Certificates'
                        },
                        {
                            href: '#',
                            text: 'Ratings'
                        },
                        {
                            href: '#',
                            text: 'Shop help'
                        },
                        {
                            href: '#',
                            text: 'Contact Us'
                        }
                    ]
                },
                {
                    title: 'Sites',
                    links: [
                        {
                            href: '#',
                            text: 'DC'
                        },
                        {
                            href: '#',
                            text: 'MAD Magazine'
                        },
                        {
                            href: '#',
                            text: 'DC Kids'
                        },
                        {
                            href: '#',
                            text: 'DC Universe'
                        },
                        {
                            href: '#',
                            text: 'DC Power Visa'
                        },
                    ]
                },
                {
                    title: 'Shop',
                    links: [
                        {
                            href: '#',
                            text: 'Shop DC'
                        },
                        {
                            href: '#',
                            text: 'Shop DC Collectibles'
                        },
                    ]
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.footer-top {
    background-image: url('@/assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;

    .logo-lg {
        background-image: url('@/assets/img/dc-logo-bg.png');
        background-position: center;
        background-repeat: no-repeat;
    }
}
</style>