<template>
  <div class="t-card">
    <img src="../../assets/images/26.jpeg" alt="Man" class="t-card__img">
    <h5 class="t-card__title">Julia Aan <span class="t-card__subtitle">- COO Sofbox</span></h5>
    <p class="t-card__text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Libero, tenetur, placeat minima aut nostrum maxime</p>
  </div>
</template>

<script>
export default {
    name: "TestimonialCard"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";
.t-card {
    width: calc(100% / 2 - 40px);
    height: 350px;
    margin: 30px 20px;
    padding: 40px 20px;
    color: $text-primary;
    border: 1px solid $border-grayscale-two;

    &__img {
        width: 80px;
        margin-bottom: 25px;
        border: 1px solid $border-light;
        border: 1px solid $border-lightblue;
        border-radius: 50%;
    }
}
</style>