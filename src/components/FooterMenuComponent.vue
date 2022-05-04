<template>
    <div class="col col-4">
        <h3>{{title}}</h3>
        <ul>
            <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{link.text}}</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'FooterMenuItem',
    props: {
        title: String,
        links: Array
    }
}
</script>

<style lang="scss" scoped>

    h3 {
        color: $lightestColor;
        text-transform: uppercase;
        padding-bottom: 1rem;
    }

    li {

        line-height: 1.5rem;

        a {
            color: $paleDarkColor;
        }
    }

</style>