<template>
  <button class="button">
    <slot/>
  </button>
</template>

<script>
export default {
    name: "Button"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.button {
    padding: 15px 25px;
    color: $text-light;
    background-color: $background-dark-blue;
    border: none;
    border-radius: 5px;
}
</style>