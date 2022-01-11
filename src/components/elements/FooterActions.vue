<template>
  <div>
      <h5>Quick Links</h5>
      <ul class="footer__links">
          <li v-for="(action, index) in  actions" :key="index">
              <a :href="action.url">{{action.text}}</a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: "FooterActions",
    props: {
        actions: Array
    }
}
</script>

<style lang="scss" scoped>

</style>