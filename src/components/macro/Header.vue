<template>
  <header class="header">
      <div class="container mt-3">
          <div class="row align-items-center">
              <div class="offset-1 col-2">
                  <img src="../../assets/images/logo-2.png" alt="Sofbox Logo" class="header__logo">
              </div>
              <div class="col-9">
                  <Navbar :links="links"/>
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
                {
                    text: "Home",
                    url: "#",
                    current: false
                },
                {
                    text: "About us",
                    url: "#",
                    current: false
                },
                {
                    text: "Feature",
                    url: "#",
                    current: false
                },
                {
                    text: "Testimonials",
                    url: "#",
                    current: false
                },
                {
                    text: "Contact US",
                    url: "#",
                    current: false
                },

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

    &__logo:hover {
        cursor: pointer;
    }
}
</style>