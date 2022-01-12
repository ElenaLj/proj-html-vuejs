<template>
  <div class="label">
      <img :src="label.img" alt="Analysis sketch" class="label__img">
      <div class="label__info">
          <h4 class="label__title">{{label.title}}</h4>
            <p class="label__text">{{label.text}}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: "Label",
    props: {
        label: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss"; 

.label {
    height: 200px;
    padding: 20px 10px;
    border: 1px solid $border-grayscale-one;
    display: flex;
    justify-content: space-between;
    align-items: center;

    &__img {
        height: 70px;
    }

    &__info {
        padding: 20px;
    }
}
</style>