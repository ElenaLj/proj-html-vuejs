<template>
    <div>
        <h5>About Us</h5>
        <ul class="footer__links">
            <li v-for="(el, index) in  elm" :key="index">
                <a :href="el.url">{{el.text}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "FooterElms",
    props: {
        elm: Array
    }
}
</script>

<style lang="scss" scoped>

</style>