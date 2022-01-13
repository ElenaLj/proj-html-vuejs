<template>
    <section class="latest">
        <div class="container">
            <div class="row">
                <div class="offset-3 col-6">
                    <h2 class="latest__title">Latest Posts</h2>
                    <p class="latest__text">If you are planning on developing a product landing.</p>
                </div>
            </div>
            <div class="latest__card">
                <Posts v-for="(post, index) in posts" :key="index" :post="post"/>
            </div>
        </div>
    </section>
</template>

<script>
import Posts from "../elements/Posts.vue";

export default {
    name: "LatestPosts",
    components: {
        Posts
    },
    data() {
        return {
            posts: 
            [
                {
                    img: require("../../assets/images/19.jpg"),
                    alt: "Graphic art",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable."
                },
                {
                    img: require("../../assets/images/18.jpg"),
                    alt: "Graphic art",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable."
                },
                {
                    img: require("../../assets/images/17.jpg"),
                    alt: "Graphic art",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.latest {
    text-align: center;

    &__card {
        display: flex;
    }
}
</style>