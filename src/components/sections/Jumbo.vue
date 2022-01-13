<template>
  <div class="container-90">
      <div class="row jumbo">
          <div class="col-5 jumbo__text">
              <h1>The biggest platform for your growth.</h1>
              <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alternation in the form</p>
              <Button>Read More</Button>
          </div>
          <div class="col-7">
              <img src="../../assets/images/27-1.png" alt="People sketch" class="jumbo__img">
          </div>
      </div>
  </div>
</template>

<script>
import Button from "../elements/Button.vue";

export default {
    name: "Jumbo",
    components: {
        Button
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.jumbo {
    padding: 70px 50px;
    max-height: 500px;
    background-color: $background-light-blue;

    &__text {
        padding-right: 20px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        gap: 30px;

        p {
            color: $text-grey;
        }
    }

    &__img {
        height: 500px;
    }
}
</style>