<template>
    <div class="posts">
        <div class="posts__item">
            <img :src="post.img" :alt="post.alt" class="posts__img">
            <h5 class="posts__title">{{post.title}}</h5>
            <p class="posts__text">{{post.text}}</p>
            <div class="posts__tag">January 12, 2022</div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Posts",
    props: {
        post: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";
.posts {
    margin: 100px 0;
    text-align: left;

    &__item {
        height: 450px;
        margin: 0 20px;
        padding: 15px;
        border: 1px solid $border-grayscale-two;
        position: relative;
    }

    &__img {
        width: 100%;
    }

    &__title {
        margin: 50px 0 18px 0;
    }

    &__text {
        color: $text-grey;
        font-weight: 500;
    }

    &__tag {
        width: fit-content;
        height: 35px;
        padding: 5px;
        color: $text-grey;
        background-color: $background-primary;
        font-size: 14px;
        font-weight: 500;
        border-radius: 5px;
        position: absolute;
        top: 25px;
        left: 25px;
    }
}
</style>