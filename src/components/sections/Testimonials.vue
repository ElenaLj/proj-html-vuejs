<template>
  <section class="testimonials">
      <div class="container">
          <div class="row">
              <div class="offset-3 col-6">
                  <h2 class="testimonials__title">Our Testimonials</h2>
                  <p class="testimonials__text">If you are planning on developing a product landind app or website, take a look at this beautiful-crafted</p>
              </div>
          </div>
          <div class="testimonials__card">
                  <TestimonialCard/>
                  <TestimonialCard/>
          </div>
      </div>
  </section>
</template>

<script>
import TestimonialCard from "../elements/TestimonialCard.vue";

export default {
    name: "Testimonials",
    components: {
        TestimonialCard
    }
}
</script>

<style lang="scss" scoped>
.testimonials {
    margin: 100px 0;
    text-align: center;

    &__card {
        display: flex;
    }
}
</style>