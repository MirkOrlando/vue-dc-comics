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
    }

    li {
        a {
            color: $paleDarkColor;
        }
    }

</style>