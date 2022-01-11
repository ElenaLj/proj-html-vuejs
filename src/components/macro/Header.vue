<template>
  <header class="header">
      <div class="container">
          <div class="row">
              <div class="col-4">
                  <img src="../../assets/images/logo-2.png" alt="Sofbox Logo" class="header__logo">
              </div>
              <div class="col-8">
                  <Navbar/>
              </div>
          </div>
      </div>

  </header>
</template>

<script>
import Navbar from "../elements/Navbar.vue";

export default {
    name: "Header",
    components: {
        Navbar
    },
    data() {
        return {
            links: 
            [
                "Home",
                "About Us",
                "Feature",
                "Testimonials",
                "Contact US"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.header {
    height: 80px;

    &__logo {
        height: 50px;
    }
}
</style>