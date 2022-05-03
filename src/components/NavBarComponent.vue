<template>
    <nav>
        <ul>
            <li v-for="(item, index) in NavItem" :key="index">{{item}}</li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'NavBarComponent',
    data() {
        return { 
            NavItem: [
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

@import '@/assets/sass/_variables.scss';

        nav {
            display: flex;
            align-items: center;
            height: 100%;
            color: $darkColor;
            ul {
                display: flex;
                height: 100%;

                li {
                    display: flex;
                    align-items: center;
                    text-transform: uppercase;
                    padding: 4rem 0;
                    margin: 0 1rem;
                    height: 100%;
                    border-bottom: 6px solid transparent;
                    font-weight: bold;

                    &.active {
                        color: $primaryColor;
                        border-color: $primaryColor;
                    }

                }
            }
        }
</style>