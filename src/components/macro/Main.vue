<template>
  <main>
    <Jumbo/>
    <OnlineMarketing/>
    <TechSupport/>
  </main>
</template>

<script>
import Jumbo from "../sections/Jumbo.vue";
import OnlineMarketing from "../sections/OnlineMarketing.vue";
import TechSupport from "../sections/TechSupport.vue";

export default {
    name: "Main",
    components: {
      Jumbo,
      OnlineMarketing,
      TechSupport
    }
}
</script>

<style lang="scss" scoped>

</style>