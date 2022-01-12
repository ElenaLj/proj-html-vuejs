<template>
  <main>
    <Jumbo/>
    <OnlineMarketing/>
    <TechSupport/>
    <FeaturesSection/>
  </main>
</template>

<script>
import Jumbo from "../sections/Jumbo.vue";
import OnlineMarketing from "../sections/OnlineMarketing.vue";
import TechSupport from "../sections/TechSupport.vue";
import FeaturesSection from "../sections/FeaturesSection.vue";

export default {
    name: "Main",
    components: {
      Jumbo,
      OnlineMarketing,
      TechSupport,
      FeaturesSection
    }
}
</script>

<style lang="scss" scoped>

</style>