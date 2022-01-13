<template>
  <div class="t-card">
    <img :src="testimonial.img" :alt="testimonial.alt" class="t-card__img">
    <h5 class="t-card__title">{{testimonial.name}} <span class="t-card__subtitle">- {{testimonial.role}}</span></h5>
    <p class="t-card__text">{{testimonial.text}}</p>
  </div>
</template>

<script>
export default {
    name: "TestimonialCard",
    props: {
      testimonial: Object
    }
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
    background-color: $background-secondary;
    box-shadow: 10px 10px 30px 10px $border-grayscale-two;
    
    &__img {
        width: 80px;
        margin-bottom: 25px;
        border: 1px solid $border-lightblue;
        border-radius: 50%;
    }

    &__subtitle {
      color: $text-grey;
      font-size: 16px;
      font-weight: 500;
    }
}
</style>