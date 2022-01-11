<template>
  <main>
    <Jumbo/>
    <OnlineMarketing/>
  </main>
</template>

<script>
import Jumbo from "../sections/Jumbo.vue";
import OnlineMarketing from "../sections/OnlineMarketing.vue";

export default {
    name: "Main",
    components: {
      Jumbo,
      OnlineMarketing
    }
}
</script>

<style lang="scss" scoped>

</style>