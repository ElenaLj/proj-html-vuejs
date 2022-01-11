<template>
  <nav class="nav-bar">
      <ul class="nav-bar__list">
          <li class="nav-bar__item" v-for="(link, index) in links" :key="index">
              <a :href="link.url">{{link.text}}</a>
          </li>
          <!-- <li class="nav-bar__item">
              <a href="#">About Us</a>
          </li>
          <li class="nav-bar__item">
              <a href="#">Feature</a>
          </li>
          <li class="nav-bar__item">
              <a href="#">Testimonials</a>
          </li>
          <li class="nav-bar__item">
              <a href="#">Contact US</a>
          </li> -->
      </ul>

      <div class="actions">
          <i class="fas fa-search actions__icon"></i>
          <i class="fas fa-shopping-cart actions__icon"></i>
          <Button>Get Started</Button>
      </div>
  </nav>
</template>

<script>
import Button from "./Button.vue";
export default {
    name: 'Navbar',
    components: {
        Button
    },
    props: {
        links: Array
    }
}
</script>

<style lang="scss" scoped>
.nav-bar {
    display: flex;

    &__list {
        margin-bottom: 0;
        margin-right: 35px;
        list-style: none;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    &__item {
        margin-right: 20px;
        
        a {
            color: inherit;
            text-decoration: none;
        }
    }

    .actions {
        > * {
            margin-right: 25px;
        }
    }
}
</style>