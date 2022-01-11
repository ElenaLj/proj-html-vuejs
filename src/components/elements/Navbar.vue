<template>
  <nav class="nav-bar">
      <ul class="nav-bar__list">
          <li class="nav-bar__item" v-for="(link, index) in links" :key="index">
              <a href="#">{{link.text}}</a>
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
  </nav>
</template>

<script>
export default {
    name: 'Navbar',
    props: {
        links: Array
    }
}
</script>

<style lang="scss" scoped>
.nav-bar {
    &__list {
        list-style: none;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    &__item {
        margin-right: 10px;
        
        a {
            color: inherit;
            text-decoration: none;
        }
    }
}
</style>