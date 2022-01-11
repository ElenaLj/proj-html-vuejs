<template>
  <section class="marketing">
      <div class="container">
          <div class="row">
            <div class="col-4">
                <Card :cards="cards"/>
            </div>

            <div class="col-4">
                <Card :cards="cards"/>
            </div>

            <div class="col-4">
                <Card :cards="cards"/>
            </div>
          </div>
      </div>
  </section>
</template>

<script>
import Card from "../elements/Card.vue";

export default {
    name: "OnlineMarketing",
    components: {
        Card
    },
    data() {
        return {
            cards: [
                "SEO",
                "SEM",
                "Website Strategy",
                "Social management"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.marketing {
    margin-top: 150px;
}
</style>