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

.button:hover {
  background-color: $background-dark;
}
</style>