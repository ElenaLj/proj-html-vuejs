<template>
  <div class="badge">
    <h6 class="badge__title">{{badge.title}}</h6>
    <img :src="badge.src" alt="Graph sketch" class="badge__img">
  </div>
</template>

<script>
export default {
    name: "Badge",
    props: {
        badge: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss"; 

.badge {
    width: calc(100% / 4 - 20px);
    margin: 10px;
    height: 180px;
    padding: 30px 20px;
    color: $text-dark;
    border: 1px solid $border-grayscale-two;
    text-align: left;

    &__title {
        font-size: 18px;
    }

    &__img {
        height: 70px;
    }
}
</style>