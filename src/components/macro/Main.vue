<template>
  <main>
    <Jumbo/>
    <OnlineMarketing/>
    <TechSupport/>
    <FeaturesSection/>
    <Testimonials/>
    <LatestPosts/>
    <Contacts/>
  </main>
</template>

<script>
import Jumbo from "../sections/Jumbo.vue";
import OnlineMarketing from "../sections/OnlineMarketing.vue";
import TechSupport from "../sections/TechSupport.vue";
import FeaturesSection from "../sections/FeaturesSection.vue";
import Testimonials from "../sections/Testimonials.vue";
import LatestPosts from "../sections/LatestPosts.vue";
import Contacts from "../sections/Contacts.vue";

export default {
    name: "Main",
    components: {
      Jumbo,
      OnlineMarketing,
      TechSupport,
      FeaturesSection,
      Testimonials,
      LatestPosts,
      Contacts
    }
}
</script>

<style lang="scss" scoped>
main {
    background-image: url(../../assets/images/14.png);
    background-repeat: no-repeat;
    background-position: -50% 40%;
}
</style>