<template>
  <main>
    <Jumbo/>
    <OnlineMarketing/>
    <TechSupport/>
    <FeaturesSection/>
    <Testimonials/>
    <LatestPosts/>
  </main>
</template>

<script>
import Jumbo from "../sections/Jumbo.vue";
import OnlineMarketing from "../sections/OnlineMarketing.vue";
import TechSupport from "../sections/TechSupport.vue";
import FeaturesSection from "../sections/FeaturesSection.vue";
import Testimonials from "../sections/Testimonials.vue";
import LatestPosts from "../sections/LatestPosts.vue";

export default {
    name: "Main",
    components: {
      Jumbo,
      OnlineMarketing,
      TechSupport,
      FeaturesSection,
      Testimonials,
      LatestPosts
    }
}
</script>

<style lang="scss" scoped>
</style>