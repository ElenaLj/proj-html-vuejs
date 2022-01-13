<template>
  <div class="socials">
    <i class="fab fa-facebook-f socials__icon"></i>
    <i class="fab fa-twitter socials__icon"></i>
    <i class="fab fa-github socials__icon"></i>
    <i class="fab fa-instagram socials__icon"></i>
  </div>
</template>

<script>
export default {
    name: "Socials"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.socials {
    display: flex;
    gap: 10px;
    margin: 50px 0;

    &__icon {
        color: $text-blue;
        padding: 15px;
        width: 50px;
        height: 50px;
        border: 1px solid $border-grayscale-two;
    }
}
</style>