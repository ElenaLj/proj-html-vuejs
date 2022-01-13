<template>
  <section class="testimonials">
      <div class="container">
          <div class="row">
              <div class="offset-3 col-6">
                  <h2 class="testimonials__title">Our Testimonials</h2>
                  <p class="testimonials__text">If you are planning on developing a product landing app or website, take a look at this beautiful-crafted</p>
              </div>
          </div>
          <div class="testimonials__card">
                  <TestimonialCard v-for="(testimonial, index) in testimonials" :key="index" :testimonial="testimonial"/>
          </div>

          <div class="testimonials__icons">
              <i class="fas fa-stop active"></i>
              <i class="fas fa-stop"></i>
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
    },
    data() {
        return {
            testimonials: 
            [
                {
                    img: require("../../assets/images/26.jpeg"),
                    alt: "Woman picture",
                    name: "Julia AAnn",
                    role: "COO Sofbox",
                    text: "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip."
                },
                {
                    img: require("../../assets/images/27.jpeg"),
                    alt: "Man picture",
                    name: "Mac Znder",
                    role: "Manager Sofbox",
                    text: "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium vero eos et consectetur accus adip adip."
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variables.scss";

.testimonials {
    margin: 150px 0;
    text-align: center;
    background-image: url(../../assets/images/15.png), linear-gradient(0deg, rgba(255,255,255,1) 33%, rgba(239,247,255,1) 64%);
    background-repeat: no-repeat;
    background-position: right -25% bottom 110%;

    &__card {
        display: flex;
        margin-top: 50px;
    }

    &__icons {
        display: flex;
        justify-content: center;

        > * {
            margin: 0 3px;
            width: 10px;
        }  

        & .active {
            color: $text-blue;
        }
    }
}
</style>