<template>
  <div>
      <h5>Menu</h5>
      <ul class="footer__links">
          <li v-for="(item, index) in  items" :key="index">
              <a :href="item.url">{{item.text}}</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: "FooterLinks",
    props: {
        items: Array
    }
}
</script>

<style lang="scss" scoped>

</style>