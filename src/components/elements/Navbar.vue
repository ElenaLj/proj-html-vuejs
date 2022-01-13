<template>
  <nav class="nav-bar">
      <ul class="nav-bar__list">
          <li class="nav-bar__item" v-for="(link, index) in links" :key="index">
              <a :href="link.url">{{link.text}}</a>
          </li>
      </ul>

      <div class="nav-bar__actions">
          <i class="fas fa-search"></i>
          <i class="fas fa-shopping-cart" id="cart"></i>
          <Button>Get Started</Button>

        <!-- shopping cart circle -->
        <div class="nav-bar__circle">0</div>
        <!-- /shopping cart circle -->
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
@import "../../assets/style/partials/variables.scss";

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
            font-weight: 500;
            text-decoration: none;
            line-height: 60px;
        }
    }

    &__item:hover {
        cursor: pointer;
        color: $text-blue;
        border-bottom: 2px solid $text-blue;
    }

    &__actions {
        position: relative;

        > * {
            margin-right: 35px;
        }
    }

    &__actions:hover {
        cursor: pointer;
    }

    &__circle {
        height: 25px;
        width: 25px;
        padding: 5px;
        text-align: center;
        line-height: 1.4;
        color: $text-light;
        font-size: 13px;
        font-weight: 500;
        background-color: $background-dark-blue;
        border-radius: 50%;
        position: absolute;
        left: 20%;
        top: 10px;
        z-index: -999;
    }
}
</style>